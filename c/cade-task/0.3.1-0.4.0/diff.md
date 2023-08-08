# Comparing `tmp/cade_task-0.3.1.tar.gz` & `tmp/cade_task-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cade_task-0.3.1.tar", max compression
+gzip compressed data, was "cade_task-0.4.0.tar", max compression
```

## Comparing `cade_task-0.3.1.tar` & `cade_task-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-06-22 21:56:01.797435 cade_task-0.3.1/LICENSE
--rw-r--r--   0        0        0     2828 2023-07-22 17:27:22.754257 cade_task-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-07-18 17:17:25.645802 cade_task-0.3.1/cade_task/__init__.py
--rw-r--r--   0        0        0       59 2023-07-22 17:27:22.754596 cade_task-0.3.1/cade_task/__main__.py
--rw-r--r--   0        0        0     3788 2023-07-22 17:27:22.754812 cade_task-0.3.1/cade_task/cli.py
--rw-r--r--   0        0        0     4235 2023-07-22 18:08:17.811586 cade_task-0.3.1/cade_task/lib.py
--rw-r--r--   0        0        0      732 2023-07-22 18:10:00.250799 cade_task-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 cade_task-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-08 03:20:58.268981 cade_task-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2828 2023-08-08 03:20:58.268981 cade_task-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 03:20:58.268981 cade_task-0.4.0/cade_task/__init__.py
+-rw-r--r--   0        0        0       59 2023-08-08 03:20:58.268981 cade_task-0.4.0/cade_task/__main__.py
+-rw-r--r--   0        0        0     4276 2023-08-08 03:20:58.268981 cade_task-0.4.0/cade_task/cli.py
+-rw-r--r--   0        0        0     4877 2023-08-08 03:20:58.268981 cade_task-0.4.0/cade_task/lib.py
+-rw-r--r--   0        0        0      756 2023-08-08 03:20:58.268981 cade_task-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 cade_task-0.4.0/PKG-INFO
```

### Comparing `cade_task-0.3.1/LICENSE` & `cade_task-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cade_task-0.3.1/README.md` & `cade_task-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cade_task-0.3.1/cade_task/cli.py` & `cade_task-0.4.0/cade_task/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from pathlib import Path
 from typing import Optional
 
 import typer
-
-# from devtools import debug  # noqa: F401
+from devtools import debug  # noqa: F401
 from rich import print
 from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
 from .lib import (
     ListNotFoundException,
@@ -100,35 +99,53 @@
 ) -> None:
     """
     Add a task to a given project
     """
     project = project_set(project, ctx.obj["project"])
     title_str = " ".join(title)
     task = TaskItem(title_str, project)
-    task.add()
-    print(f"Task '{title_str}' added to {project}.")
+    new_task = task.add()
+    print(f":white_check_mark: Task '{new_task.title}' added to {new_task.parent}.")
+
+
+@app.command()
+def edit(
+    ctx: typer.Context,
+    index: int,
+    title: list[str],
+    project: Annotated[Optional[str], typer.Option("--list")] = None,
+) -> None:
+    """
+    Add a task to a given project
+    """
+    project = project_set(project, ctx.obj["project"])
+    title_str = " ".join(title)
+    task = TaskItem(title_str, project, index=index)
+    task.edit()
+    print(
+        f":white_check_mark: Task {index} modified to '{task.title}' in {task.parent}."
+    )
 
 
 @app.command()
 def complete(
     ctx: typer.Context,
     tasks: list[str],
     project: Annotated[Optional[str], typer.Option("--list")] = None,
 ) -> None:
     """
     Complete task(s) for a given project
     """
     project = project_set(project, ctx.obj["project"])
 
     for t in sorted(tasks, reverse=True):
-        # FIXME: setting a dummy title is inelegant
         task = TaskItem(title="complete_task", parent=project, index=int(t))
         task.complete()
 
-    print("Task(s) completed.")
+    print(":white_check_mark: Task(s) completed.")
 
 
 @app.command()
 def open() -> None:
     """
     Open Reminders.app or move it to the foreground
     """
```

### Comparing `cade_task-0.3.1/cade_task/lib.py` & `cade_task-0.4.0/cade_task/lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from dataclasses import dataclass
 from pathlib import Path
 from shutil import which
 from subprocess import CalledProcessError, run
 from typing import Any
 
-# from devtools import debug  # noqa: F401
+from devtools import debug  # noqa: F401
 
 
 @dataclass
 class TaskItem(object):
     """Reminder/task"""
 
     title: str
@@ -30,23 +30,24 @@
 
         for attribute in task.copy():
             if attribute in rename_rules:
                 task[rename_rules[attribute]] = task.pop(attribute)
 
         return TaskItem(**task)
 
-    def add(self):
-        # Successful output: Added 'yet another test' to 'test'
-        run_and_return(["add", self.parent, self.title])
+    def add(self) -> "TaskItem":
+        result = run_and_return(["add", self.parent, self.title], mode="json")
+        task = TaskItem.from_dict(result.output)
+        return task
 
     def complete(self):
         run_and_return(["complete", self.parent, str(self.index)])
 
     def edit(self):
-        pass
+        run_and_return(["edit", self.parent, self.index, self.title], mode="raw")
 
 
 @dataclass
 class TaskList:
     """Reminders list object"""
 
     name: str
@@ -64,15 +65,16 @@
             run_and_return(["new-list", self.name], mode="raw")
 
     def tasks(self) -> list[TaskItem] | None:
         if hasattr(self, "_tasks"):
             return self._tasks  # type: ignore
 
         try:
-            tasks = run_and_return(["show", self.name], mode="json")
+            result = run_and_return(["show", self.name], mode="json")
+            tasks = result.output
         except TaskCommandException as e:
             if "No reminders list matching" in e.output:
                 raise ListNotFoundException(f"List '{self.name}' not found")
             else:
                 raise
 
         self._tasks = [TaskItem.from_dict(t) for t in tasks]  # type: ignore[arg-type]
@@ -100,41 +102,59 @@
     if len(parts) >= 1:
         project = parts[0]
 
     return project
 
 
 def get_lists() -> list[str]:
-    return run_and_return(["show-lists"], mode="json")
+    result = run_and_return(["show-lists"], mode="json")
+    return result.output
+
+
+@dataclass
+class RunAndReturnResult:
+    command: str
+    # FIXME: Unions, mypy, and I aren't friends
+    # output: list[str | dict[str, Any]] | dict[str, Any]
+    output: Any
+    unmarshalled_output: bytes
+    return_code: int
 
 
 def run_and_return(
     cmd: list[str], mode: str = "raw", inject_reminder: bool = True
-) -> list[str]:
+) -> RunAndReturnResult:
     # Add reminders path to beginning of command
     if inject_reminder:
         cmd = [reminders()] + cmd
 
     if mode == "json":
         cmd = cmd + ["--format", "json"]
 
     try:
         result = run(cmd, capture_output=True, check=True, shell=False)
     except CalledProcessError as e:
         raise TaskCommandException(e)
 
     if mode == "raw":
-        raw = result.stdout.decode("utf-8").splitlines()
-        return raw
+        marshalled_result = result.stdout.decode("utf-8").splitlines()
     elif mode == "json":
-        json_output = result.stdout.decode("utf-8").strip()
-        return json.loads(json_output)
+        result_output = result.stdout.decode("utf-8").strip()
+        marshalled_result = json.loads(result_output)
     else:
         raise TaskException("invalid mode")
 
+    result_obj = RunAndReturnResult(
+        command=" ".join(result.args),
+        output=marshalled_result,
+        unmarshalled_output=result.stdout,
+        return_code=result.returncode,
+    )
+    return result_obj
+
 
 def reminders() -> str:
     reminders = which("reminders")
     if not reminders:
         raise TaskException("reminders-cli not found")
     return reminders
```

### Comparing `cade_task-0.3.1/pyproject.toml` & `cade_task-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cade-task"
-version = "0.3.1"
+version = "0.4.0"
 description = "A loose wrapper around reminders-cli"
 readme = "README.md"
 authors = ["Cade Ekblad-Frank <cade@e-f.me>"]
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/cadeef/cade-task"
 
@@ -20,14 +20,15 @@
 pytest = "^7.4.0"
 black = "^23.7.0"
 ruff = "^0.0.278"
 mypy = "^1.4.1"
 devtools = "^0.11.0"
 pygments = "^2.15.1"
 coveralls = "^3.3.1"
+pytest-mock = "^3.11.1"
 
 [build-system]
 requires = ["poetry>=1.5.1"]
 build-backend = "poetry.masonry.api"
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/rules/
```

### Comparing `cade_task-0.3.1/PKG-INFO` & `cade_task-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cade-task
-Version: 0.3.1
+Version: 0.4.0
 Summary: A loose wrapper around reminders-cli
 Author: Cade Ekblad-Frank
 Author-email: cade@e-f.me
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
```

