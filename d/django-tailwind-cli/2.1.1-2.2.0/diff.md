# Comparing `tmp/django_tailwind_cli-2.1.1.tar.gz` & `tmp/django_tailwind_cli-2.2.0.tar.gz`

## Comparing `django_tailwind_cli-2.1.1.tar` & `django_tailwind_cli-2.2.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/mkdocs.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/base_template.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/changelog.md
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/development.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/index.md
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/installation.md
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/settings.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/template_tags.md
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/docs/usage.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/__version__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/settings.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/test_management_commands.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/test_tailwind_css_tag.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/LICENSE
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/README.md
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 django_tailwind_cli-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/mkdocs.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/CNAME
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/base_template.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/changelog.md
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/development.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/index.md
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/installation.md
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/settings.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/template_tags.md
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/__version__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/settings.py
+-rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/test_management_commands.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/test_tailwind_css_tag.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/README.md
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/PKG-INFO
```

### Comparing `django_tailwind_cli-2.1.1/.pre-commit-config.yaml` & `django_tailwind_cli-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/CHANGELOG.md` & `django_tailwind_cli-2.2.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 2.2.0
+
+- [#49](https://github.com/oliverandrich/django-tailwind-cli/pull/49) by [@andrlik](https://github.com/andrlik) added a new management command `tailwind list_templates`.
+- The new default config uses this command to implent the idea of Calton Gibson outlined in his blog post [Using Django’s template loaders to configure Tailwind](https://noumenal.es/notes/tailwind/django-integration/).
+
 ## 2.1.1
 
 - Switched from poetry to hatch for package management.
 
 ## 2.0.6
 
 - Bugfix for default tailwind.config.js.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_tailwind_cli-2.1.1/mkdocs.yml` & `django_tailwind_cli-2.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/.github/workflows/publish.yml` & `django_tailwind_cli-2.2.0/.github/workflows/publish.yml`

 * *Files 25% similar despite different names*

```diff
@@ -19,24 +19,18 @@
 
       - name: Ensure latest pip
         run: python -m pip install --upgrade pip
 
       - name: Install hatch
         run: python -m pip install hatch
 
-      - name: Configure hatch
-        run: hatch config set "dirs.env.virtual" ".venv"
-
       - name: Built
         run: hatch build
 
       - name: Publish
         env:
           HATCH_INDEX_USER: "__token__"
           HATCH_INDEX_AUTH: "${{ secrets.PYPI_TOKEN }}"
         run: hatch publish
 
       - name: Deploy docs
-        uses: mhausenblas/mkdocs-deploy-gh-pages@master
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-          CUSTOM_DOMAIN: django-tailwind-cli.andrich.me
+        run: hatch run docs:deploy
```

### Comparing `django_tailwind_cli-2.1.1/.github/workflows/test.yml` & `django_tailwind_cli-2.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/docs/base_template.md` & `django_tailwind_cli-2.2.0/docs/base_template.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/docs/development.md` & `django_tailwind_cli-2.2.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/docs/installation.md` & `django_tailwind_cli-2.2.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/docs/template_tags.md` & `django_tailwind_cli-2.2.0/docs/template_tags.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/docs/usage.md` & `django_tailwind_cli-2.2.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-2.2.0/src/django_tailwind_cli/utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/src/django_tailwind_cli/management/commands/tailwind.py` & `django_tailwind_cli-2.2.0/src/django_tailwind_cli/management/commands/tailwind.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """`tailwind` management command."""
 
+import os
 import shutil
 import ssl
 import subprocess
 import sys
 import urllib.request
 from multiprocessing import Process
-from typing import Any, List
+from pathlib import Path
+from typing import Any, List, Union
 
 import certifi
 from django.conf import settings
 from django.core.management.base import BaseCommand, CommandError
+from django.template.utils import get_app_template_dirs
 
 from django_tailwind_cli.utils import Config
 
 
 class Command(BaseCommand):
     """Create and manage a Tailwind CSS theme."""
 
@@ -35,14 +38,16 @@
         """Add arguments to the command."""
         subparsers = parser.add_subparsers(dest="tailwind", required=True)
 
         subparsers.add_parser("build", help="Build a minified production ready CSS file.")
 
         subparsers.add_parser("watch", help="Start Tailwind CLI in watch mode during development.")
 
+        subparsers.add_parser("list_templates", help="List the templates of your django project.")
+
         runserver_parser = subparsers.add_parser(
             "runserver", help="Start the Django development server and the Tailwind CLI in watch mode."
         )
         runserver_parser.add_argument("addrport", nargs="?", help="Optional port number, or ipaddr:port")
 
     def handle(self, *_args: Any, **kwargs: Any) -> None:
         """Perform the command's actions."""
@@ -59,14 +64,16 @@
         # Start the subcommand.
         if label == "build":
             self.build()
         elif label == "watch":
             self.watch()
         elif label == "runserver":  # pragma: no cover
             self.runserver(**kwargs)
+        elif label == "list_templates":
+            self.list_templates()
 
     def build(self) -> None:
         """Build a minified production ready CSS file."""
         try:
             subprocess.run(self.get_build_cmd(), cwd=settings.BASE_DIR, check=True)  # noqa: S603
         except KeyboardInterrupt:
             self.stdout.write(self.style.ERROR("Canceled building production stylesheet."))
@@ -114,14 +121,31 @@
             debugserver_process.start()
             watch_process.join()
             debugserver_process.join()
         except KeyboardInterrupt:
             watch_process.terminate()
             debugserver_process.terminate()
 
+    def list_templates(self):
+        template_files: List[str] = []
+        app_template_dirs = get_app_template_dirs("templates")
+        for app_template_dir in app_template_dirs:
+            template_files += self.list_template_files(app_template_dir)
+        template_files += self.list_template_files(settings.TEMPLATES[0]["DIRS"])
+
+        self.stdout.write("\n".join(template_files))
+
+    def list_template_files(self, template_dir: Union[str, Path]) -> List[str]:
+        template_files: List[str] = []
+        for dirpath, _, filenames in os.walk(str(template_dir)):
+            for filename in filenames:
+                if filename.endswith(".html") or filename.endswith(".txt"):
+                    template_files.append(os.path.join(dirpath, filename))
+        return template_files
+
     def get_build_cmd(self) -> List[str]:
         """Get the command to build the CSS."""
         if self.config.src_css is None:
             return [
                 str(self.config.get_full_cli_path()),
                 "--output",
                 str(self.config.get_full_dist_css_path()),
@@ -180,20 +204,43 @@
             self.stdout.write(self.style.ERROR("Tailwind CSS config not found."))
             tailwind_config_file.write_text(DEFAULT_TAILWIND_CONFIG)
             self.stdout.write(self.style.SUCCESS(f"Created Tailwind CSS config at '{tailwind_config_file}'"))
 
 
 DEFAULT_TAILWIND_CONFIG = """/** @type {import('tailwindcss').Config} */
 const plugin = require("tailwindcss/plugin");
+const { spawnSync } = require('child_process');
+
+// Calls Django to fetch template files
+const getTemplateFiles = () => {
+    const command = 'python3';
+    const args = ['-m', 'django', 'list_templates'];
+    // Assumes tailwind.config.js is located in the BASE_DIR of your Django project.
+    const options = { cwd: __dirname };
+
+    const result = spawnSync(command, args, options);
+
+    if (result.error){
+        throw result.error;
+    }
+
+    if (result.status !== 0){
+        console.log(result.stdout.toString(), result.stderr.toString());
+        throw new Error(`Django management command exited with code ${result.status}`);
+    }
+
+    const templateFiles = result.stdout.toString()
+        .split('\n')
+        .map((file) => file.trim())
+        .filter(function(e){return e}); // Remove empty strings, including last empty line.
+    return templateFiles;
+}
 
 module.exports = {
-  content: [
-    './templates/**/*.html',
-    '**/templates/**/*.html',
-  ],
+  content: [].concat(getTemplateFiles()),
   theme: {
     extend: {},
   },
   plugins: [
     require('@tailwindcss/typography'),
     require('@tailwindcss/forms'),
     require('@tailwindcss/aspect-ratio'),
```

### Comparing `django_tailwind_cli-2.1.1/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-2.2.0/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/tests/settings.py` & `django_tailwind_cli-2.2.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/tests/test_management_commands.py` & `django_tailwind_cli-2.2.0/tests/test_management_commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,15 +61,16 @@
 class BasicManagementCommandFunctionalityTestCase(MockedNetworkingProcessesAndShellToolsTestCase):
     """Test the basic functionality of all management commands."""
 
     def test_calling_unknown_subcommand(self):
         """Unknown subcommands to the tailwind management command raise a `CommandError`."""
 
         with self.assertRaisesRegex(
-            CommandError, r"invalid choice: 'notavalidcommand' \(choose from 'build', 'watch', 'runserver'\)"
+            CommandError,
+            r"invalid choice: 'notavalidcommand' \(choose from 'build', 'watch', 'list_templates', 'runserver'\)",
         ):
             with captured_output():
                 call_command("tailwind", "notavalidcommand")
 
     def test_invalid_configuration(self):
         """An invalid configuration raises a `CommandError`."""
 
@@ -202,14 +203,43 @@
         self.assertNotIn("--input", build_cmd)
 
         with self.settings(TAILWIND_CLI_SRC_CSS="css/source.css"):
             build_cmd = TailwindCommand().get_watch_cmd()
             self.assertIn("--input", build_cmd)
 
 
+class ListTemplateCommandTestCase(MockedNetworkingProcessesAndShellToolsTestCase):
+    """Test that list_templates command works."""
+
+    def test_list_project_templates(self):
+        """Test that the list_templates command returns our two templates."""
+        with captured_output() as (out, _err):
+            call_command("tailwind", "list_templates")
+        self.assertIn("templates/tailwind_cli/base.html", out.getvalue().strip())
+        self.assertIn("templates/tailwind_cli/tailwind_css.html", out.getvalue().strip())
+        self.assertNotIn("templates/admin", out.getvalue().strip())
+
+    def test_list_all_templates(self):
+        """Test that app templates are also included."""
+        admin_installed_apps = [
+            "django.contrib.contenttypes",
+            "django.contrib.messages",
+            "django.contrib.auth",
+            "django.contrib.admin",
+            "django.contrib.staticfiles",
+            "django_tailwind_cli",
+        ]
+        with self.settings(INSTALLED_APPS=admin_installed_apps):
+            with captured_output() as (out, _err):
+                call_command("tailwind", "list_templates")
+        self.assertIn("templates/admin", out.getvalue().strip())
+        self.assertIn("templates/tailwind_cli/base.html", out.getvalue().strip())
+        self.assertIn("templates/tailwind_cli/tailwind_css.html", out.getvalue().strip())
+
+
 @contextmanager
 def captured_output():
     """Capture the output of a function."""
 
     new_out, new_err = StringIO(), StringIO()
     old_out, old_err = sys.stdout, sys.stderr
     try:
```

### Comparing `django_tailwind_cli-2.1.1/tests/test_tailwind_css_tag.py` & `django_tailwind_cli-2.2.0/tests/test_tailwind_css_tag.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/tests/test_utils.py` & `django_tailwind_cli-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/.gitignore` & `django_tailwind_cli-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/LICENSE` & `django_tailwind_cli-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/README.md` & `django_tailwind_cli-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.1.1/pyproject.toml` & `django_tailwind_cli-2.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,23 +40,31 @@
 
 # Default environment
 [tool.hatch.envs.default]
 dependencies = ["django-types"]
 
 # Test environment
 [[tool.hatch.envs.test.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
-django = ["3.2", "4.1", "4.2"]
+python = ["3.8", "3.9", "3.10"]
+django = ["3.2"]
+
+[[tool.hatch.envs.test.matrix]]
+python = ["3.8", "3.9", "3.10", "3.11"]
+django = ["4.1", "4.2"]
+
+[[tool.hatch.envs.test.matrix]]
+python = ["3.12"]
+django = ["4.2"]
 
 [tool.hatch.envs.test]
 dependencies = ["django-rich", "coverage[toml]", "django~={matrix:django}.0"]
 
 [tool.hatch.envs.test.scripts]
-test = "python -m django test --settings tests.settings"
-test-cov = "coverage run -m django test --settings tests.settings"
+test = "python -m django test --settings tests.settings {args}"
+test-cov = "coverage run -m django test --settings tests.settings {args}"
 cov-report = ["coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
 
 # Lint environment
 [tool.hatch.envs.lint]
 dependencies = ["pyright", "django-types", "curlylint", "black", "ruff"]
 
@@ -72,14 +80,15 @@
 # Docs environment
 [tool.hatch.envs.docs]
 dependencies = ["mkdocs-material"]
 
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --clean --strict"
 serve = "mkdocs serve"
+deploy = "mkdocs gh-deploy"
 
 # Black
 [tool.black]
 target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
```

### Comparing `django_tailwind_cli-2.1.1/PKG-INFO` & `django_tailwind_cli-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 2.1.1
+Version: 2.2.0
 Summary: Django and Tailwind integration based on the prebuilt Tailwind CSS CLI.
 Project-URL: Documentation, https://django-tailwind-cli.andrich.me/
 Project-URL: Issues, https://github.com/oliverandrich/django-tailwind-cli/issues
 Project-URL: Source, https://github.com/oliverandrich/django-tailwind-cli
 Author-email: Oliver Andrich <oliver@andrich.me>
 License-Expression: MIT
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.1.1 Summary: Django
+Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.2.0 Summary: Django
 and Tailwind integration based on the prebuilt Tailwind CSS CLI. Project-URL:
 Documentation, https://django-tailwind-cli.andrich.me/ Project-URL: Issues,
 https://github.com/oliverandrich/django-tailwind-cli/issues Project-URL:
 Source, https://github.com/oliverandrich/django-tailwind-cli Author-email:
 Oliver Andrich
 andrich.me> License-Expression: MIT License-File: LICENSE Keywords:
 css,django,tailwind Classifier: Development Status :: 5 - Production/Stable
```

