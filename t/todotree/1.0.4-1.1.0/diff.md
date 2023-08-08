# Comparing `tmp/todotree-1.0.4.tar.gz` & `tmp/todotree-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todotree-1.0.4.tar", max compression
+gzip compressed data, was "todotree-1.1.0.tar", max compression
```

## Comparing `todotree-1.0.4.tar` & `todotree-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-07-30 09:39:41.168573 todotree-1.0.4/LICENSE
--rw-r--r--   0        0        0     1855 2023-07-30 09:39:41.168573 todotree-1.0.4/README.md
--rw-r--r--   0        0        0     2169 2023-07-30 09:40:02.068727 todotree-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      196 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Errors/ProjectFolderError.py
--rw-r--r--   0        0        0      180 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Errors/TaskParseError.py
--rw-r--r--   0        0        0      198 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Errors/WishListFolderError.py
--rw-r--r--   0        0        0        0 2023-07-30 09:39:41.204573 todotree-1.0.4/todotree/Errors/__init__.py
--rw-r--r--   0        0        0    12425 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Task.py
--rw-r--r--   0        0        0    11122 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Taskmanager.py
--rw-r--r--   0        0        0     4493 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/Tree.py
--rw-r--r--   0        0        0        0 2023-07-30 09:39:41.204573 todotree-1.0.4/todotree/__init__.py
--rw-r--r--   0        0        0     5960 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/config.py
--rwxr-xr-x   0        0        0    10611 2023-07-30 09:39:41.174573 todotree-1.0.4/todotree/main.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 todotree-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-08-08 09:35:59.169535 todotree-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1855 2023-08-08 09:35:59.169535 todotree-1.1.0/README.md
+-rw-r--r--   0        0        0     2195 2023-08-08 09:36:19.552707 todotree-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-08-08 09:35:59.174535 todotree-1.1.0/todotree/Errors/ConfigFileNotFound.py
+-rw-r--r--   0        0        0      132 2023-08-08 09:35:59.174535 todotree-1.1.0/todotree/Errors/DoneFileNotFound.py
+-rw-r--r--   0        0        0      118 2023-08-08 09:35:59.174535 todotree-1.1.0/todotree/Errors/ProjectFolderError.py
+-rw-r--r--   0        0        0      102 2023-08-08 09:35:59.174535 todotree-1.1.0/todotree/Errors/TaskParseError.py
+-rw-r--r--   0        0        0      132 2023-08-08 09:35:59.174535 todotree-1.1.0/todotree/Errors/TodoFileNotFound.py
+-rw-r--r--   0        0        0      124 2023-08-08 09:35:59.174535 todotree-1.1.0/todotree/Errors/WishListFolderError.py
+-rw-r--r--   0        0        0        0 2023-08-08 09:35:59.199535 todotree-1.1.0/todotree/Errors/__init__.py
+-rw-r--r--   0        0        0    12425 2023-08-08 09:35:59.175535 todotree-1.1.0/todotree/Task.py
+-rw-r--r--   0        0        0    11713 2023-08-08 09:35:59.175535 todotree-1.1.0/todotree/Taskmanager.py
+-rw-r--r--   0        0        0     4493 2023-08-08 09:35:59.175535 todotree-1.1.0/todotree/Tree.py
+-rw-r--r--   0        0        0        0 2023-08-08 09:35:59.199535 todotree-1.1.0/todotree/__init__.py
+-rw-r--r--   0        0        0     6071 2023-08-08 09:35:59.175535 todotree-1.1.0/todotree/config.py
+-rwxr-xr-x   0        0        0    13952 2023-08-08 09:35:59.175535 todotree-1.1.0/todotree/main.py
+-rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 todotree-1.1.0/PKG-INFO
```

### Comparing `todotree-1.0.4/LICENSE` & `todotree-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `todotree-1.0.4/README.md` & `todotree-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `todotree-1.0.4/pyproject.toml` & `todotree-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "todotree"
-version = "1.0.4"
+version = "1.1.0"
 description = "todo.txt manager which adds tree printing"
 authors = ["chim1aap <fkjansen@protonmail.com>"]
 repository = "https://gitlab.com/chim1aap/todotree"
 documentation = "https://chim1aap.gitlab.io/todotree/"
 readme = "README.md"
 packages = [
   {include = "todotree"}
@@ -14,17 +14,18 @@
     "README.md",
     "dist/*.zsh",
     "dist/*.bash",
     "dist/*.fish"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.10,<4.0"
 click = "^8.1.3"
 gitpython = "^3.1.31"
+xdg-base-dirs = "^6.0.0"
 
 [tool.poetry.group.dev.dependencies]
 requests = "^2.28.2, !=2.30.0"
 coverage = "^7.2.7"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.6.4"
```

### Comparing `todotree-1.0.4/todotree/Task.py` & `todotree-1.1.0/todotree/Task.py`

 * *Files identical despite different names*

### Comparing `todotree-1.0.4/todotree/Taskmanager.py` & `todotree-1.1.0/todotree/Taskmanager.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import os
 import pathlib
 import re
 import shutil
 from tempfile import (  # https://docs.python.org/3/library/tempfile.html
     NamedTemporaryFile,
 )
-
+from todotree.Errors.TodoFileNotFound import TodoFileNotFound
+from todotree.Errors.DoneFileNotFound import DoneFileNotFound
 from todotree.Errors.ProjectFolderError import ProjectFolderError
 from todotree.Errors.WishListFolderError import WishListFolderError
 from todotree.Task import Task
 from todotree.Tree import Tree
 from todotree.config import Config
 
 # regexes
@@ -81,22 +82,25 @@
             self._import_projecttree_folder()
 
     def _import_from_todo_txt(self):
         """
         Imports the todos from the file to the Taskmanager object.
         :return:
         """
-        with open(self.config.todofile, 'r') as f:
-            content = f.readlines()
-            self.task_list = []
-            for i, task in enumerate(content):
-                # Skip empty lines.
-                if task.strip() == "":
-                    continue
-                self.task_list.append(Task(i + 1, task.strip()))
+        try:
+            with open(self.config.todofile, 'r') as f:
+                content = f.readlines()
+                self.task_list = []
+                for i, task in enumerate(content):
+                    # Skip empty lines.
+                    if task.strip() == "":
+                        continue
+                    self.task_list.append(Task(i + 1, task.strip()))
+        except FileNotFoundError as e:
+            raise TodoFileNotFound from e
 
     def filter_t_date(self):
         """
         Removes Tasks from the Taskmanager where the t:date is later than today.
         """
         start_list = self.task_list.copy()  # Iterable copy.
         for task in start_list:
@@ -154,16 +158,16 @@
         """
         try:
             wishlist_items = os.listdir(self.config.wishlist_folder)
             for item in wishlist_items:
                 wish_task = Task(0, item)
                 wish_task.projects.append(self.config.wishlistName)
                 self.task_list.append(wish_task)
-        except FileNotFoundError:
-            raise WishListFolderError("An Error occurred while processing the Wishlist Folder.")
+        except FileNotFoundError as e:
+            raise WishListFolderError("An Error occurred while processing the Wishlist Folder.") from e
 
     #  readonly methods.
 
     def __str__(self):
         self.task_list.sort(key=lambda x: x.priority)
         s = self.config.consoleGood + " Todos\n"
         number_of_digits = int(math.ceil(math.log(len(self.task_list) + 1, 10)))
@@ -179,16 +183,19 @@
         return s
 
     def list_done(self):
         """
         List the done.txt with numbers to revive them.
         :return:
         """
-        with open(self.config.donefile, "r") as f:
-            lines = f.readlines()
+        try:
+            with open(self.config.donefile, "r") as f:
+                lines = f.readlines()
+        except FileNotFoundError as e:
+            raise DoneFileNotFound from e
         for i, line in reversed(list(enumerate(lines))):
             print(i, line, end="")
 
     def filter_by_string(self, filter_string):
         """
         Filters the task list by whether `filter_string` occurred in the task.
         """
@@ -221,21 +228,24 @@
         """
         Write the results back to a file.
         :return:
         """
         # Write to new file.
         self.task_list.sort(key=lambda x: x.i)
         #  Delete=false is needed for windows, I hope that somebodies temp folder won't be clobbered with this..
-        with NamedTemporaryFile("w+t", newline="", delete=False) as temp_file:
-            # may strip new lines by using task list.
-            for n in self.task_list:
-                temp_file.write(str(n.raw_string))
-                temp_file.write("\n")
-            temp_file.flush()
-            shutil.copy(temp_file.name, self.config.todofile)
+        try:
+            with NamedTemporaryFile("w+t", newline="", delete=False) as temp_file:
+                # may strip new lines by using task list.
+                for n in self.task_list:
+                    temp_file.write(str(n.raw_string))
+                    temp_file.write("\n")
+                temp_file.flush()
+                shutil.copy(temp_file.name, self.config.todofile)
+        except FileNotFoundError as e:
+            raise TodoFileNotFound from e
 
     def change_t_date(self, date, task_number):
         """
         Adds or changes the t:date
         :param date: The new t:date to add.
         :param task_number: The task number to add the new date to.
         :return: The updated task.
@@ -255,33 +265,25 @@
         :return:
         """
         tsk = self.task_list[task_number - 1]
         tsk.update_priority(priority)
         self.write_todo_to_file()
         return tsk
 
-    @staticmethod
-    def append_line_to_file(line, file):
-        """
-        Append line to a file
-        :param line:
-        :param file:
-        :return:
-        """
-        f = open(file, "a")
-        f.write(line)
-        f.close()
-
-    def add_task(self, tsk):
+    def add_task_to_file(self, tsk: str):
         """
         Adds a task to a file. Returns the task with its assigned number.
         :param tsk:
         :return:
         """
-        self.append_line_to_file(tsk, self.config.todofile)
+        try:
+            with open(self.config.todofile, 'a') as f:
+                f.write(tsk)
+        except FileNotFoundError as e:
+            raise TodoFileNotFound from e
         # return the line number
         return len(self.task_list) + 1
 
     def append_to_task(self, task_number: int, task_string: str) -> str:
         """
         Appends :param task_string: to :param task_number:
         It :return: the result.
@@ -305,27 +307,33 @@
             completed_tasks.append(self.task_list[num - 1])
             del self.task_list[num - 1]
         # Save the new task list.
         self.write_todo_to_file()
         # Convert completed tasks to done tasks.
         done_tasks = map(lambda x: task_to_done(x), completed_tasks)
         # Append the results to done.txt
-        with open(self.config.donefile, "a") as f:
-            for completed_task in done_tasks:
-                f.write(completed_task + "\n")
+        try:
+            with open(self.config.donefile, "a") as f:
+                for completed_task in done_tasks:
+                    f.write(completed_task + "\n")
+        except FileNotFoundError as e:
+            raise DoneFileNotFound from e
         return done_tasks
 
     def revive_task(self, line_number):
         """
         Gets task from done.txt and adds it to the task file.
         The task does not get removed.
         :param line_number:
         :return:
         """
         # Fetch Task
-        with open(self.config.donefile) as f:
-            done_tasks = f.readlines()
+        try:
+            with open(self.config.donefile) as f:
+                done_tasks = f.readlines()
+        except FileNotFoundError as e:
+            raise DoneFileNotFound from e
         tsk = done_tasks[line_number - 1]
         tsk = task_to_undone(tsk)
         # Add task
-        self.add_task(tsk)
+        self.add_task_to_file(tsk)
         return tsk
```

### Comparing `todotree-1.0.4/todotree/Tree.py` & `todotree-1.1.0/todotree/Tree.py`

 * *Files identical despite different names*

### Comparing `todotree-1.0.4/todotree/config.py` & `todotree-1.1.0/todotree/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,48 @@
-import os
-import pathlib
 from pathlib import Path
 
+import xdg_base_dirs as xdg
 import yaml
 
+from todotree.Errors import ConfigFileNotFound
+
 
 class Config:
     """
     The configuration of todotree.
     """
     def __init__(self):
         #  Main variables.
-        self.todo_folder: Path = Path("./")
+        self.todo_folder: Path = xdg.xdg_data_home() / "todotree"
         """
-        Path to the folder containing the configuration.
-
-        Relative paths are relative to the main.py file, not to the todo.txt file.
+        Path to the folder containing the data files.
+        
+        Relative paths are calculated from the HOME folder. 
         """
 
-        self.project_tree_folder: Path = os.getenv("TODOTXT_PROJECTTREE_FOLDER", pathlib.Path.home())
+        self.project_tree_folder: Path = xdg.xdg_data_home() / "todotree" / "projects"
         """
         Path to the folder containing the projects.
-        Defaults to the home directory if not set.
+        Defaults to the XDG_DATA_DIR/todotree/projects if not set.
         """
 
-        self.wishlist_folder: Path = os.getenv("TODOTXT_WISHLIST_FOLDER", pathlib.Path.home())
+        self.wishlist_folder: Path = xdg.xdg_data_home() / "todotree" / "wishlists"
         """
         Path to the folder containing the wishlist items.
-        Defaults to the home directory if not set.
+        Defaults to XDG_DATA_DIR/todotree/wishlist if not set.
+        """
+
+        self.todofile = Path(self.todo_folder) / "todo.txt"
+        """
+        Path to the todo.txt file.
+        """
+
+        self.donefile = Path(self.todo_folder) / "done.txt"
+        """
+        Path to the done.txt file.
         """
 
         self.git_mode = "None"
         """The mode that git runs in. 
         - None disables it,
         - Local add and commits, 
         - Full also pushes it to a remote repo.
@@ -59,38 +70,30 @@
         self.extendedGood = ' Notice:'
         self.extendedWarn = ' Warning:'
         self.extendedError = ' Error:'
 
         #  Status Decorators.
 
         self.consoleGood: str = ' * '
-        self.consoleWarn: str = "\033[33m *\033[0m"
-        self.consoleError: str = '\033[31m *\033[0m'
+        self.consoleWarn: str = ' ! '
+        self.consoleError: str = '!!!'
 
         # Tree prints.
         self.t_print: str = " ├──"
         self.l_print: str = " │  "
         self.s_print: str = " └──"
         self.e_print: str = "    "
 
-        # Non trivial.
-        self.todofile = Path(self.todo_folder) / "todo.txt"
-        """
-        Path to the todo.txt file.
-        """
-
-        self.donefile = Path(self.todo_folder) / "done.txt"
-        """
-        Path to the done.txt file.
-        """
-
     def read_from_file(self, file: Path):
         """Reads and parses yaml content from `file`."""
-        with open(file, 'r') as f:
-            self.read_from_yaml(f.read())
+        try:
+            with open(file, 'r') as f:
+                self.read_from_yaml(f.read())
+        except FileNotFoundError as e:
+            raise ConfigFileNotFound from e
 
     def read_from_yaml(self, yaml_content: str):
         """Reads and overrides config settings defined in `yaml_content`."""
         # Convert yaml to python object.
         yaml_object = yaml.safe_load(yaml_content)
         if yaml_object is None:
             return
```

### Comparing `todotree-1.0.4/todotree/main.py` & `todotree-1.1.0/todotree/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import re
 import subprocess
 from pathlib import Path
 from typing import List
 
 import click  # CLI magic
 from git import Repo
+
+from todotree.Errors.TodoFileNotFound import TodoFileNotFound
+from todotree.Errors.DoneFileNotFound import DoneFileNotFound
+from todotree.Errors.ConfigFileNotFound import ConfigFileNotFound
 from todotree.Taskmanager import Taskmanager, task_to_done
 from todotree.config import Config
 
 
 # Click Replaces:
 # Argparse
 #
@@ -30,66 +34,115 @@
     """todotree main help."""
     # ^ This text also shows up in the help command.
     # Root click group. This manages all the command line interactions.
     # ensure that ctx.obj exists and is a dict
     self.ensure_object(dict)
     # parsing arguments.
     config = Config()
-    if config_path is not None:
-        config.read_from_file(config_path)
+    try:
+        if config_path is not None:
+            config.read_from_file(config_path)
+    except ConfigFileNotFound as e:
+        handle_config_file_not_found(e, self, config_path)
+
     if todo_file is not None:
         config.todofile = todo_file
     if done_file is not None:
         config.donefile = done_file
+
     # creating variables a la __init__.
     self.obj["config"] = config
     self.obj["task_manager"] = Taskmanager(configuration=config)
     # Pass to another command.
     pass
 
 
+def handle_config_file_not_found(e, self, config_path):
+    """Handle when a """
+    click.echo(self.obj["config"].consoleWarn + " The config.yaml file could not be found.")
+    if self.obj["config"].verbose:
+        click.echo(f"The config file should be located at {config_path}")
+        click.echo(e)
+    click.echo("The default options are now used.")
+
+
 @root.command('add', short_help='Add a task to the task list')
 @click.argument('task', type=str)  # , short_help = 'Task To Add')
 @click.pass_context
 def add(self, task: str):
-    self.obj["task_manager"].add_task(task.strip() + "\n")
-    commit_exit("add", self.obj["config"])
+    try:
+        self.obj["task_manager"].add_task_to_file(task.strip() + "\n")
+        commit_exit("add", self.obj["config"])
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
+
+
+def handle_todo_file_not_found(e, self):
+    """Inform the user that the todo.txt was not found."""
+    click.echo(f"{self.obj['config'].consoleError} The todo.txt could not be found.")
+    click.echo(
+        f"{self.obj['config'].consoleError} It searched at the following location: {self.obj['config'].todofile}")
+    if self.obj["config"].verbose:
+        click.echo(e)
 
 
 @root.command('addx', short_help='Add a task and immediately mark it as done')
 @click.argument('task', type=str)
 @click.pass_context
 def add_x(self, task):
-    f = open(self.obj["config"].donefile, "a")
-    done = task_to_done(
-        task.strip())
-    f.write(done)
-    click.echo(done)
+    try:
+        f = open(self.obj["config"].donefile, "a")
+        done = task_to_done(
+            task.strip())
+        f.write(done)
+        click.echo(done)
+    except FileNotFoundError as e:
+        handle_done_file_not_found(e, self)
+        exit(1)
+
+
+def handle_done_file_not_found(e, self):
+    """Inform the user that the done.txt was not found."""
+    click.echo(self.obj["config"].consoleError + " The done.txt could not be found.")
+    click.echo(
+        f"{self.obj['config'].consoleError} It searched at the following location: {self.obj['config'].donefile}")
+    if self.obj["config"].verbose:
+        click.echo(e)
 
 
 @root.command('append', short_help='append append_string to task_nr')
 @click.argument('task_nr', type=int)
 @click.argument('append_string')
 @click.pass_context
 def append(self, task_nr: int, append_string: str):
     # Disable fancy imports, because they are not needed.
     self.obj['config'].enable_project_folder = False
     self.obj['config'].enable_wishlist_folder = False
     # Import tasks.
-    self.obj["task_manager"].import_tasks()
+    try:
+        self.obj["task_manager"].import_tasks()
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
+
     click.echo(self.obj["task_manager"].append_to_task(task_nr, append_string.strip()))
     commit_exit("append", self.obj["config"])
 
 
 @root.command('context',
               short_help='list task in a tree, by context',
               help='list a tree, of which the first node is the context, the second nodes are the tasks')
 @click.pass_context
 def context(self):
-    self.obj['task_manager'].import_tasks()
+    try:
+        self.obj['task_manager'].import_tasks()
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
     # Print due tree.
     click.echo(self.obj['task_manager'].print_context_tree())
     exit()
 
 
 @root.command('cd',
               short_help='print directory of the todo.txt directory',
@@ -100,15 +153,15 @@
     config_path: Path = Path(self.obj['config'].todo_folder)
 
     if config_path.is_absolute():
         # Then the configured path is printed.
         click.echo(os.path.dirname(config_path))
         exit()
     # Then the relative path is resolved to be absolute.
-    base_path: Path = os.path.realpath(__file__)
+    base_path: Path = Path.home()
     full_path: Path = base_path / config_path
     click.echo(os.path.dirname(full_path))
     exit()
 
 
 @root.command('do',
               short_help='mark task as done and move it to the done.txt'
@@ -118,16 +171,24 @@
 def do(self, task_numbers: List[str]):
     # Convert to ints.
     task_numbers = [int(i) for i in task_numbers]
     # Marking something as Done cannot be done with fancy imports
     # So we disable them.
     self.obj['config'].enable_project_folder = False
     self.obj['config'].enable_wishlist_folder = False
-    self.obj['task_manager'].import_tasks()
-    completed_tasks = self.obj["task_manager"].mark_as_done(task_numbers)
+    try:
+        self.obj['task_manager'].import_tasks()
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
+    try:
+        completed_tasks = self.obj["task_manager"].mark_as_done(task_numbers)
+    except DoneFileNotFound as e:
+        handle_done_file_not_found(e, self)
+        exit(1)
     # Print the results
     click.echo(self.obj['config'].consoleGood + " Tasks marked as done:")
     click.echo(completed_tasks)
     commit_exit("do", self.obj["config"])
 
 
 @root.command('due',
@@ -135,15 +196,19 @@
               )
 @click.pass_context
 def due(self):
     # Disable fancy imports, because they do not have due dates.
     self.obj['config'].enable_project_folder = False
     self.obj['config'].enable_wishlist_folder = False
     # Import tasks.
-    self.obj['task_manager'].import_tasks()
+    try:
+        self.obj['task_manager'].import_tasks()
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
     # Print due tree.
     click.echo(self.obj['task_manager'].print_by_due())
     exit()
 
 
 @root.command('edit',
               short_help='open the todo.txt in $EDITOR (or nano)'
@@ -162,90 +227,130 @@
 
 @root.command('filter',
               short_help='only show tasks containing the search term.'
               )
 @click.argument('search_term')
 @click.pass_context
 def filter_list(self, search_term):
-    self.obj["task_manager"].import_tasks()
+    try:
+        self.obj["task_manager"].import_tasks()
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
     self.obj["task_manager"].filter_by_string(search_term)
     click.echo(self.obj["task_manager"])
 
 
 @root.command('list', short_help='List tasks')
 @click.pass_context
 def list_tasks(self):
-    self.obj["task_manager"].import_tasks()
+    try:
+        self.obj["task_manager"].import_tasks()
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
     click.echo(self.obj["task_manager"])
 
 
 @root.command('list_done', short_help='List tasks which are marked as done')
 @click.pass_context
 def list_done(self):
-    self.obj["task_manager"].list_done()
+    try:
+        self.obj["task_manager"].list_done()
+    except DoneFileNotFound as e:
+        handle_done_file_not_found(e, self)
+        exit(1)
 
 
 @root.command('print_raw', short_help='print todo.txt without any formatting or filtering')
 @click.pass_context
 def print_raw(self):
     try:
         with open(self.obj["task_manager"].config.todofile, "r") as f:
             click.echo(f.read())
-    except FileNotFoundError:
-        click.echo(self.obj["config"].consoleError + "File Not Found")
+    except FileNotFoundError as e:
+        handle_todo_file_not_found(e, self)
 
 
 @root.command('priority', short_help='set new priority to task')
 @click.argument('task_number', type=int)
 @click.argument('new_priority', type=str)
 @click.pass_context
 def priority(self, task_number, new_priority):
     # Disable fancy imports.
     self.obj['config'].enable_project_folder = False
     self.obj['config'].enable_wishlist_folder = False
     # Run task.
-    self.obj["task_manager"].import_tasks()
+    try:
+        self.obj["task_manager"].import_tasks()
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
     self.obj["task_manager"].change_priority(
         priority=(new_priority.upper()), task_number=task_number)
 
 
 @root.command('project', short_help='print tree by project')
 @click.pass_context
 def project(self):
     # Import tasks.
-    self.obj['task_manager'].import_tasks()
+    try:
+        self.obj["task_manager"].import_tasks()
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
     # Print due tree.
     click.echo(self.obj['task_manager'].print_project_tree())
     exit()
 
 
 @root.command('revive', short_help='Revive a task that was accidentally marked as done.')
 @click.argument('done_number', type=int)
 @click.pass_context
 def revive(self, done_number):
-    click.echo(self.obj["task_manager"].revive_task(done_number))
+    try:
+        click.echo(self.obj["task_manager"].revive_task(done_number))
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
+    except DoneFileNotFound as e:
+        handle_done_file_not_found(e, self)
+        exit(1)
     commit_exit("revive", self.obj["config"])
 
 
 @root.command('schedule', short_help='hide task until date.',
               help='hide the task until the date given. If new_date is not in ISO format (yyyy-mm-dd), '
                    'then it tries to figure out the date with the `date` program, which is only in linux.'
               )
 @click.pass_context
+@click.argument('task_number', type=int)
+@click.argument('new_date', type=str)
 def schedule(self, task_number, new_date):
+    # Disable fancy imports, because they do not have t dates.
+    self.obj['config'].enable_project_folder = False
+    self.obj['config'].enable_wishlist_folder = False
+
     date = " ".join(new_date)
     date_pattern = re.compile(r"(\d{4})-(\d{2})-(\d{2})")
     if not date_pattern.match(date):
+        # Try to use the `date` utility.
         dat = subprocess.run(
             ["date", "-d " + date, "+%F "],
             capture_output=True,
             encoding="utf-8"
         )
         date = dat.stdout.strip()
-    self.obj["task_manager"].change_t_date(date, task_number)
+    try:
+        self.obj["task_manager"].import_tasks()
+        self.obj["task_manager"].change_t_date(date, task_number)
+    except TodoFileNotFound as e:
+        handle_todo_file_not_found(e, self)
+        exit(1)
+
     commit_exit("schedule", self.obj["config"])
 
 
 @root.group()
 @click.pass_context
 def stale():
     """
@@ -314,15 +419,15 @@
     Commit the files with git before exiting.
 
     :param config: The configuration parameters.
     :param action: The name of the action, such as list or add.
     """
     if config.git_mode != "Local":
         exit()
-    repo = Repo(Config.todo_folder)
+    repo = Repo(config.todo_folder)
 
     # Git add.
     repo.index.add('*')
 
     # Git commit.
     time = datetime.datetime.now().isoformat()
     repo.index.commit(message=time + action)
```

### Comparing `todotree-1.0.4/PKG-INFO` & `todotree-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: todotree
-Version: 1.0.4
+Version: 1.1.0
 Summary: todo.txt manager which adds tree printing
 Home-page: https://gitlab.com/chim1aap/todotree
 Author: chim1aap
 Author-email: fkjansen@protonmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
+Requires-Dist: xdg-base-dirs (>=6.0.0,<7.0.0)
 Project-URL: Documentation, https://chim1aap.gitlab.io/todotree/
 Project-URL: Repository, https://gitlab.com/chim1aap/todotree
 Description-Content-Type: text/markdown
 
 # todotree
 
 [![Release](https://img.shields.io/gitlab/v/release/chim1aap/todotree)](https://img.shields.io/gitlab/v/release/chim1aap/todotree)
```

