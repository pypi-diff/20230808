# Comparing `tmp/dup_hawk-0.0.7.tar.gz` & `tmp/dup_hawk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dup_hawk-0.0.7.tar", max compression
+gzip compressed data, was "dup_hawk-0.0.9.tar", max compression
```

## Comparing `dup_hawk-0.0.7.tar` & `dup_hawk-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1059 2023-07-23 18:21:31.109104 dup_hawk-0.0.7/LICENSE
--rw-r--r--   0        0        0     1246 2023-07-23 18:21:31.109104 dup_hawk-0.0.7/README.md
--rw-r--r--   0        0        0      126 2023-07-23 18:21:31.109104 dup_hawk-0.0.7/dup_hawk/__init__.py
--rw-r--r--   0        0        0     4405 2023-07-23 18:21:31.109104 dup_hawk-0.0.7/dup_hawk/dup_hawk.py
--rw-r--r--   0        0        0     2475 2023-07-23 18:21:31.109104 dup_hawk-0.0.7/dup_hawk/github.py
--rw-r--r--   0        0        0      667 2023-07-23 18:21:31.109104 dup_hawk-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 dup_hawk-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-08-08 02:26:50.181176 dup_hawk-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1711 2023-08-08 02:26:50.181176 dup_hawk-0.0.9/README.md
+-rw-r--r--   0        0        0      126 2023-08-08 02:26:50.181176 dup_hawk-0.0.9/dup_hawk/__init__.py
+-rw-r--r--   0        0        0     5490 2023-08-08 02:26:50.181176 dup_hawk-0.0.9/dup_hawk/dup_hawk.py
+-rw-r--r--   0        0        0     2875 2023-08-08 02:26:50.181176 dup_hawk-0.0.9/dup_hawk/github.py
+-rw-r--r--   0        0        0      668 2023-08-08 02:26:50.185176 dup_hawk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 dup_hawk-0.0.9/PKG-INFO
```

### Comparing `dup_hawk-0.0.7/LICENSE` & `dup_hawk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dup_hawk-0.0.7/README.md` & `dup_hawk-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 # dup_hawk
 
 🦅 A bot the looks for duplicate issues on a GitHub repo, created especially for competitive security reviews. 
 
+<!-- use html to import an image -->
+<p align="center">
+  <img src="./img/dups.png" alt="dup-hawk" width="500"/>
+</p>
+
+
 # Getting Started
 ## Requirements
 
 - [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
   - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
 - [Python](https://www.python.org/downloads/)
   - You'll know you've installed python right if you can run:
     - `python --version` or `python3 --version` and get an output like: `Python x.x.x`
 - [pipx](https://pypa.github.io/pipx/installation/)
   - `pipx` is different from [pip](https://pypi.org/project/pip/)
   - You may have to close and re-open your terminal
   - You'll know you've installed it right if you can run:
     - `pipx --version` and see something like `x.x.x.x`
+- [poetry](https://python-poetry.org/docs/)
+  - You'll know you've installed it right if you can run `poetry --version` and get an output like `Poetry (version 1.4.2)`
 
 ## Installation
 
 ### pipx
 
 ```
 pipx install dup_hawk
@@ -33,19 +41,22 @@
 ```
 
 ## Quickstart 
 
 ```
 dup-hawk --help
 ```
-will output:
 
-```
+To run the duplicate checker, run:
 
 ```
+dup-hawk --git-repo-url {URL} --git-pat-token {PAT_TOKEN}
+```
+
+And you will have marked the issues on your github repo!
 
 # Tests
 
 ```
 poetry run pytest
 ```
 
@@ -55,8 +66,12 @@
 poetry run pytest -m ""
 ```
 
 ## Specific tests with pdb and stdout
 
 ```
 poetry run pytest -k "test_mark_duplicates_from_dfs" --pdb -s
-```
+```
+
+# Big TODO
+
+Add mocking unit tests.
```

### Comparing `dup_hawk-0.0.7/dup_hawk/github.py` & `dup_hawk-0.0.9/dup_hawk/github.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
-from typing import Optional
+import logging as log
+from typing import List, Optional
 from urllib.parse import urlparse
 
 import requests
 
+log.basicConfig(level=log.INFO)
+
 BASE_URL = "https://api.github.com/"
 X_GITHUB_API_VERSION = "2022-11-28"
 HEADERS = {
     "Accept": "application/vnd.github+json",
     "Authorization": "token ",
     "X-GitHub-Api-Version": X_GITHUB_API_VERSION,
 }
+PER_PAGE = 100
 
 
 class Github:
     def __init__(self, token: str):
         self.token = token
         self.headers = HEADERS
         self.headers["Authorization"] = f"token {self.token}"
@@ -27,30 +31,38 @@
 
     def get_repo(self, repo_url: str) -> dict:
         owner, repo = self.get_owner_and_repo(repo_url)
         url = self.url + f"repos/{owner}/{repo}"
         response = requests.get(url, headers=self.headers)
         return response.json()
 
-    def get_issues(self, repo_url: str, state: Optional[str] = "open") -> dict:
+    def get_issues(self, repo_url: str, state: Optional[str] = "open") -> List[dict]:
         """
         Gets a list of issues for a given repo.
 
         Args:
             repo_url (str): The repo to get issues from
             state (str, optional): Can be one of [open, closed, all]. Defaults to open.
 
         Returns:
             dict: _description_
         """
         owner, repo = self.get_owner_and_repo(repo_url)
         url = self.url + f"repos/{owner}/{repo}/issues"
-        params = {"state": state}
-        response = requests.get(url, headers=self.headers, params=params)
-        return response.json()
+        page_index = 1
+        results = []
+        while True:
+            params = {"state": state, "per_page": PER_PAGE, "page": page_index}
+            log.info(f"Getting page {page_index} of issues for {repo_url}")
+            response = requests.get(url, headers=self.headers, params=params)
+            if len(response.json()) == 0:
+                break
+            results.extend(response.json())
+            page_index += 1
+        return results
 
     def tag_issue(self, issue_number: int, repo_url: str, labels: list[str]) -> dict:
         owner, repo = self.get_owner_and_repo(repo_url)
         url = self.url + f"repos/{owner}/{repo}/issues/{issue_number}/labels"
         data = {"labels": labels}
         response = requests.post(url, headers=self.headers, data=json.dumps(data))
         if response.status_code > 399:
```

### Comparing `dup_hawk-0.0.7/pyproject.toml` & `dup_hawk-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "dup-hawk"
-version = "0.0.7"
+version = "0.0.9"
 description = "Python CLI for marking duplicates submissions on GitHub."
 authors = ["PatrickAlphac <54278053+PatrickAlphaC@users.noreply.github.com>"]
 readme = "README.md"
-packages = [{include = "dup_hawk"}]
+packages = [{ include = "dup_hawk" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 click = "^8.1.4"
 pytest = "^7.4.0"
 python-dotenv = "^1.0.0"
 requests = "^2.31.0"
@@ -21,8 +21,8 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-dup-hawk = 'dup_hawk.dup_hawk:dup_hawk_click'  
+dup-hawk = 'dup_hawk.dup_hawk:dup_hawk_click'
```

### Comparing `dup_hawk-0.0.7/PKG-INFO` & `dup_hawk-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dup-hawk
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python CLI for marking duplicates submissions on GitHub.
 Author: PatrickAlphac
 Author-email: 54278053+PatrickAlphaC@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,27 +20,35 @@
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # dup_hawk
 
 🦅 A bot the looks for duplicate issues on a GitHub repo, created especially for competitive security reviews. 
 
+<!-- use html to import an image -->
+<p align="center">
+  <img src="./img/dups.png" alt="dup-hawk" width="500"/>
+</p>
+
+
 # Getting Started
 ## Requirements
 
 - [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
   - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
 - [Python](https://www.python.org/downloads/)
   - You'll know you've installed python right if you can run:
     - `python --version` or `python3 --version` and get an output like: `Python x.x.x`
 - [pipx](https://pypa.github.io/pipx/installation/)
   - `pipx` is different from [pip](https://pypi.org/project/pip/)
   - You may have to close and re-open your terminal
   - You'll know you've installed it right if you can run:
     - `pipx --version` and see something like `x.x.x.x`
+- [poetry](https://python-poetry.org/docs/)
+  - You'll know you've installed it right if you can run `poetry --version` and get an output like `Poetry (version 1.4.2)`
 
 ## Installation
 
 ### pipx
 
 ```
 pipx install dup_hawk
@@ -55,19 +63,22 @@
 ```
 
 ## Quickstart 
 
 ```
 dup-hawk --help
 ```
-will output:
 
-```
+To run the duplicate checker, run:
 
 ```
+dup-hawk --git-repo-url {URL} --git-pat-token {PAT_TOKEN}
+```
+
+And you will have marked the issues on your github repo!
 
 # Tests
 
 ```
 poetry run pytest
 ```
 
@@ -78,7 +89,12 @@
 ```
 
 ## Specific tests with pdb and stdout
 
 ```
 poetry run pytest -k "test_mark_duplicates_from_dfs" --pdb -s
 ```
+
+# Big TODO
+
+Add mocking unit tests. 
+
```

