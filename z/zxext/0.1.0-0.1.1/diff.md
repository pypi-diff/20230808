# Comparing `tmp/zxext-0.1.0.tar.gz` & `tmp/zxext-0.1.1.tar.gz`

## Comparing `zxext-0.1.0.tar` & `zxext-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 zxext-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zxext-0.1.0/src/zxext/Url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zxext-0.1.0/src/zxext/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zxext-0.1.0/src/zxext/models.py
--rw-r--r--   0        0        0    12317 2020-02-02 00:00:00.000000 zxext-0.1.0/src/zxext/workbook.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 zxext-0.1.0/src/zxext/.vscode/settings.json
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 zxext-0.1.0/LICENSE
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 zxext-0.1.0/README.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 zxext-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 zxext-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      506 2020-02-02 00:00:00.000000 zxext-0.1.1/package.bat
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 zxext-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zxext-0.1.1/src/zxext/.gitattributes
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zxext-0.1.1/src/zxext/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 zxext-0.1.1/src/zxext/README.md
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zxext-0.1.1/src/zxext/Url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zxext-0.1.1/src/zxext/__init__.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 zxext-0.1.1/src/zxext/models.py
+-rw-r--r--   0        0        0    12352 2020-02-02 00:00:00.000000 zxext-0.1.1/src/zxext/workbook.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 zxext-0.1.1/src/zxext/.vscode/settings.json
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 zxext-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 zxext-0.1.1/README.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 zxext-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 zxext-0.1.1/PKG-INFO
```

### Comparing `zxext-0.1.0/src/zxext/models.py` & `zxext-0.1.1/src/zxext/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,8 +51,17 @@
 @dataclass
 class Knowledge:
     id: str
     name: str
     isChild: bool
     '''是否为子知识'''
     parentKnowledgeId: str
-    '''如果是，上一级的知识ID'''
+    '''如果是，上一级的知识ID'''
+
+@dataclass
+class TextBookChapter:
+    chapterId: str = None
+    '''教科书章节的编号'''
+    chapterName: str = None
+    '''章节名'''
+    chapterType: str = None 
+    '''本章节的类型，有unit和course'''
```

### Comparing `zxext-0.1.0/src/zxext/workbook.py` & `zxext-0.1.1/src/zxext/workbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from typing import List
 from requests import Session
 from zhixuewang.models import (
     Subject,
-    TextBook,
+    TextBook
+)
+from zxext.models import (
+    Question, 
+    QuestionDifficulty, 
+    QuestionKnowledges, 
+    QuestionSection, 
+    Knowledge, 
     TextBookChapter
 )
-from zxext.models import Question, QuestionDifficulty, QuestionKnowledges, QuestionSection, Knowledge
 from zxext.Url import Urls as Url
 
 class Workbook:
     _session: Session = None
     def __init__(self, teacherSession):
         self._session = teacherSession
     def get_problems(
```

### Comparing `zxext-0.1.0/LICENSE` & `zxext-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zxext-0.1.0/pyproject.toml` & `zxext-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
-requires = ["hatchling", "zhixuewang==1.1.11", "requests"]
+requires = ["hatchling", "zhixuewang==1.1.12", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zxext"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="MasterYuan418" },
 ]
 description = "zhixuewang库的扩展包"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/MasterYuan418/zhixue-ext"
-"Bug Tracker" = "https://github.com/MasterYuan418/zhixue-ext/issues"
+"Homepage" = "https://github.com/MasterYuan418/zxext"
+"Bug Tracker" = "https://github.com/MasterYuan418/zxext/issues"
```

