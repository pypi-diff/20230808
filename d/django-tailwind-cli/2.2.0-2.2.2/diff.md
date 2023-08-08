# Comparing `tmp/django_tailwind_cli-2.2.0.tar.gz` & `tmp/django_tailwind_cli-2.2.2.tar.gz`

## Comparing `django_tailwind_cli-2.2.0.tar` & `django_tailwind_cli-2.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/mkdocs.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/CNAME
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/base_template.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/changelog.md
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/development.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/index.md
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/installation.md
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/settings.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/template_tags.md
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/docs/usage.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/__version__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/settings.py
--rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/test_management_commands.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/test_tailwind_css_tag.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/LICENSE
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/README.md
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/mkdocs.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/docs/CNAME
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/docs/base_template.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/docs/changelog.md
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/docs/development.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/docs/index.md
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/docs/installation.md
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/docs/settings.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/docs/template_tags.md
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/docs/usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/__version__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     9542 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/tests/settings.py
+-rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/tests/test_management_commands.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/tests/test_tailwind_css_tag.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/tests/test_utils.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/LICENSE
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/README.md
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 django_tailwind_cli-2.2.2/PKG-INFO
```

### Comparing `django_tailwind_cli-2.2.0/.pre-commit-config.yaml` & `django_tailwind_cli-2.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/CHANGELOG.md` & `django_tailwind_cli-2.2.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## 2.2.2
+
+- Fixed an error locating templates from the global template directories configured via `settings.TEMPLATES[0]["DIRS"]`.
+
+## 2.2.1
+
+- Fixed a bug introduced by refactoring the changes from [#49](https://github.com/oliverandrich/django-tailwind-cli/pull/49).
+
 ## 2.2.0
 
 - [#49](https://github.com/oliverandrich/django-tailwind-cli/pull/49) by [@andrlik](https://github.com/andrlik) added a new management command `tailwind list_templates`.
 - The new default config uses this command to implent the idea of Calton Gibson outlined in his blog post [Using Django’s template loaders to configure Tailwind](https://noumenal.es/notes/tailwind/django-integration/).
 
 ## 2.1.1
```

### Comparing `django_tailwind_cli-2.2.0/mkdocs.yml` & `django_tailwind_cli-2.2.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/.github/workflows/publish.yml` & `django_tailwind_cli-2.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/.github/workflows/test.yml` & `django_tailwind_cli-2.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/docs/base_template.md` & `django_tailwind_cli-2.2.2/docs/base_template.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/docs/development.md` & `django_tailwind_cli-2.2.2/docs/development.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/docs/installation.md` & `django_tailwind_cli-2.2.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/docs/settings.md` & `django_tailwind_cli-2.2.2/docs/settings.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 /** @type {import('tailwindcss').Config} */
 const plugin = require("tailwindcss/plugin");
 const { spawnSync } = require("child_process");
 
 // Calls Django to fetch template files
 const getTemplateFiles = () => {
   const command = "python3";
-  const args = ["-m", "django", "list_templates"];
+  const args = ["-m", "django", "tailwind", "list_templates"];
   // Assumes tailwind.config.js is located in the BASE_DIR of your Django project.
   const options = { cwd: __dirname };
 
   const result = spawnSync(command, args, options);
 
   if (result.error) {
     throw result.error;
```

### Comparing `django_tailwind_cli-2.2.0/docs/template_tags.md` & `django_tailwind_cli-2.2.2/docs/template_tags.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/docs/usage.md` & `django_tailwind_cli-2.2.2/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-2.2.2/src/django_tailwind_cli/utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/src/django_tailwind_cli/management/commands/tailwind.py` & `django_tailwind_cli-2.2.2/src/django_tailwind_cli/management/commands/tailwind.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,17 @@
             debugserver_process.terminate()
 
     def list_templates(self):
         template_files: List[str] = []
         app_template_dirs = get_app_template_dirs("templates")
         for app_template_dir in app_template_dirs:
             template_files += self.list_template_files(app_template_dir)
-        template_files += self.list_template_files(settings.TEMPLATES[0]["DIRS"])
+
+        for template_dir in settings.TEMPLATES[0]["DIRS"]:
+            template_files += self.list_template_files(template_dir)
 
         self.stdout.write("\n".join(template_files))
 
     def list_template_files(self, template_dir: Union[str, Path]) -> List[str]:
         template_files: List[str] = []
         for dirpath, _, filenames in os.walk(str(template_dir)):
             for filename in filenames:
@@ -204,53 +206,58 @@
             self.stdout.write(self.style.ERROR("Tailwind CSS config not found."))
             tailwind_config_file.write_text(DEFAULT_TAILWIND_CONFIG)
             self.stdout.write(self.style.SUCCESS(f"Created Tailwind CSS config at '{tailwind_config_file}'"))
 
 
 DEFAULT_TAILWIND_CONFIG = """/** @type {import('tailwindcss').Config} */
 const plugin = require("tailwindcss/plugin");
-const { spawnSync } = require('child_process');
+const { spawnSync } = require("child_process");
 
 // Calls Django to fetch template files
 const getTemplateFiles = () => {
-    const command = 'python3';
-    const args = ['-m', 'django', 'list_templates'];
-    // Assumes tailwind.config.js is located in the BASE_DIR of your Django project.
-    const options = { cwd: __dirname };
-
-    const result = spawnSync(command, args, options);
-
-    if (result.error){
-        throw result.error;
-    }
-
-    if (result.status !== 0){
-        console.log(result.stdout.toString(), result.stderr.toString());
-        throw new Error(`Django management command exited with code ${result.status}`);
-    }
-
-    const templateFiles = result.stdout.toString()
-        .split('\n')
-        .map((file) => file.trim())
-        .filter(function(e){return e}); // Remove empty strings, including last empty line.
-    return templateFiles;
-}
+  const command = "python3";
+  const args = ["-m", "django", "tailwind", "list_templates"];
+  // Assumes tailwind.config.js is located in the BASE_DIR of your Django project.
+  const options = { cwd: __dirname };
+
+  const result = spawnSync(command, args, options);
+
+  if (result.error) {
+    throw result.error;
+  }
+
+  if (result.status !== 0) {
+    console.log(result.stdout.toString(), result.stderr.toString());
+    throw new Error(
+      `Django management command exited with code ${result.status}`
+    );
+  }
+
+  const templateFiles = result.stdout
+    .toString()
+    .split("\n")
+    .map((file) => file.trim())
+    .filter(function (e) {
+      return e;
+    }); // Remove empty strings, including last empty line.
+  return templateFiles;
+};
 
 module.exports = {
   content: [].concat(getTemplateFiles()),
   theme: {
     extend: {},
   },
   plugins: [
-    require('@tailwindcss/typography'),
-    require('@tailwindcss/forms'),
-    require('@tailwindcss/aspect-ratio'),
-    require('@tailwindcss/container-queries'),
+    require("@tailwindcss/typography"),
+    require("@tailwindcss/forms"),
+    require("@tailwindcss/aspect-ratio"),
+    require("@tailwindcss/container-queries"),
     plugin(function ({ addVariant }) {
       addVariant("htmx-settling", ["&.htmx-settling", ".htmx-settling &"]);
       addVariant("htmx-request", ["&.htmx-request", ".htmx-request &"]);
       addVariant("htmx-swapping", ["&.htmx-swapping", ".htmx-swapping &"]);
       addVariant("htmx-added", ["&.htmx-added", ".htmx-added &"]);
     }),
   ],
-}
+};
 """
```

### Comparing `django_tailwind_cli-2.2.0/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-2.2.2/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/tests/settings.py` & `django_tailwind_cli-2.2.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/tests/test_management_commands.py` & `django_tailwind_cli-2.2.2/tests/test_management_commands.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/tests/test_tailwind_css_tag.py` & `django_tailwind_cli-2.2.2/tests/test_tailwind_css_tag.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/tests/test_utils.py` & `django_tailwind_cli-2.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/.gitignore` & `django_tailwind_cli-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/LICENSE` & `django_tailwind_cli-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/README.md` & `django_tailwind_cli-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/pyproject.toml` & `django_tailwind_cli-2.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.2.0/PKG-INFO` & `django_tailwind_cli-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 2.2.0
+Version: 2.2.2
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
-Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.2.0 Summary: Django
+Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.2.2 Summary: Django
 and Tailwind integration based on the prebuilt Tailwind CSS CLI. Project-URL:
 Documentation, https://django-tailwind-cli.andrich.me/ Project-URL: Issues,
 https://github.com/oliverandrich/django-tailwind-cli/issues Project-URL:
 Source, https://github.com/oliverandrich/django-tailwind-cli Author-email:
 Oliver Andrich
 andrich.me> License-Expression: MIT License-File: LICENSE Keywords:
 css,django,tailwind Classifier: Development Status :: 5 - Production/Stable
```

