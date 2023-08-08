# Comparing `tmp/acl_anthology_py-0.1.0.tar.gz` & `tmp/acl_anthology_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acl_anthology_py-0.1.0.tar", max compression
+gzip compressed data, was "acl_anthology_py-0.2.0.tar", max compression
```

## Comparing `acl_anthology_py-0.1.0.tar` & `acl_anthology_py-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,32 @@
--rw-r--r--   0        0        0    11358 2023-05-29 13:56:57.095957 acl_anthology_py-0.1.0/LICENSE
--rw-r--r--   0        0        0      577 2023-05-29 15:53:45.069492 acl_anthology_py-0.1.0/LICENSE.header
--rw-r--r--   0        0        0     1357 2023-05-29 16:16:42.695312 acl_anthology_py-0.1.0/README.md
--rw-r--r--   0        0        0      653 2023-05-29 15:53:45.069492 acl_anthology_py-0.1.0/acl_anthology/__init__.py
--rw-r--r--   0        0        0      970 2023-05-29 15:53:45.069492 acl_anthology_py-0.1.0/acl_anthology/anthology.py
--rw-r--r--   0        0        0      818 2023-05-29 15:53:45.069492 acl_anthology_py-0.1.0/acl_anthology/logging.py
--rw-r--r--   0        0        0      650 2023-05-29 15:53:45.069492 acl_anthology_py-0.1.0/acl_anthology/papers/__init__.py
--rw-r--r--   0        0        0     1670 2023-05-29 15:53:45.069492 acl_anthology_py-0.1.0/acl_anthology/papers/index.py
--rw-r--r--   0        0        0     3391 2023-05-29 15:53:45.069492 acl_anthology_py-0.1.0/acl_anthology/utils.py
--rw-r--r--   0        0        0     1379 2023-05-29 16:58:21.184630 acl_anthology_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2666 1970-01-01 00:00:00.000000 acl_anthology_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-22 10:29:16.938162 acl_anthology_py-0.2.0/LICENSE
+-rw-r--r--   0        0        0      577 2023-05-29 19:15:49.150178 acl_anthology_py-0.2.0/LICENSE.header
+-rw-r--r--   0        0        0     3809 2023-08-08 12:45:08.746835 acl_anthology_py-0.2.0/README.md
+-rw-r--r--   0        0        0      696 2023-07-19 16:57:39.161763 acl_anthology_py-0.2.0/acl_anthology/__init__.py
+-rw-r--r--   0        0        0     4619 2023-08-07 17:39:56.344376 acl_anthology_py-0.2.0/acl_anthology/anthology.py
+-rw-r--r--   0        0        0      813 2023-07-19 16:57:39.150763 acl_anthology_py-0.2.0/acl_anthology/collections/__init__.py
+-rw-r--r--   0        0        0     3663 2023-08-07 12:05:25.397434 acl_anthology_py-0.2.0/acl_anthology/collections/collection.py
+-rw-r--r--   0        0        0     2646 2023-08-07 13:11:47.021462 acl_anthology_py-0.2.0/acl_anthology/collections/index.py
+-rw-r--r--   0        0        0    13600 2023-08-07 12:24:32.769130 acl_anthology_py-0.2.0/acl_anthology/collections/paper.py
+-rw-r--r--   0        0        0     7825 2023-08-07 17:35:06.941577 acl_anthology_py-0.2.0/acl_anthology/collections/volume.py
+-rw-r--r--   0        0        0     1809 2023-08-07 12:02:16.866361 acl_anthology_py-0.2.0/acl_anthology/config.py
+-rw-r--r--   0        0        0      739 2023-07-19 16:57:39.933761 acl_anthology_py-0.2.0/acl_anthology/constants.py
+-rw-r--r--   0        0        0     4069 2023-07-24 11:40:13.677609 acl_anthology_py-0.2.0/acl_anthology/data/schema.rnc
+-rw-r--r--   0        0        0   216411 2023-07-04 09:03:15.918345 acl_anthology_py-0.2.0/acl_anthology/data/unimathsymbols.txt
+-rw-r--r--   0        0        0     2057 2023-08-07 15:54:19.718982 acl_anthology_py-0.2.0/acl_anthology/exceptions.py
+-rw-r--r--   0        0        0     3248 2023-07-24 11:40:13.677609 acl_anthology_py-0.2.0/acl_anthology/files.py
+-rw-r--r--   0        0        0      767 2023-08-07 09:59:43.309259 acl_anthology_py-0.2.0/acl_anthology/people/__init__.py
+-rw-r--r--   0        0        0    11849 2023-08-07 18:35:10.572542 acl_anthology_py-0.2.0/acl_anthology/people/index.py
+-rw-r--r--   0        0        0     6190 2023-08-07 15:12:49.286904 acl_anthology_py-0.2.0/acl_anthology/people/name.py
+-rw-r--r--   0        0        0     2470 2023-08-07 14:24:25.770400 acl_anthology_py-0.2.0/acl_anthology/people/person.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:06:59.861920 acl_anthology_py-0.2.0/acl_anthology/py.typed
+-rw-r--r--   0        0        0      703 2023-07-04 09:03:15.919345 acl_anthology_py-0.2.0/acl_anthology/text/__init__.py
+-rw-r--r--   0        0        0     5168 2023-08-07 17:51:11.120321 acl_anthology_py-0.2.0/acl_anthology/text/markuptext.py
+-rw-r--r--   0        0        0    10736 2023-08-07 12:06:49.993463 acl_anthology_py-0.2.0/acl_anthology/text/texmath.py
+-rw-r--r--   0        0        0     1050 2023-08-07 12:03:23.535390 acl_anthology_py-0.2.0/acl_anthology/utils/__init__.py
+-rw-r--r--   0        0        0     4437 2023-06-26 13:06:59.861920 acl_anthology_py-0.2.0/acl_anthology/utils/ids.py
+-rw-r--r--   0        0        0     1520 2023-07-19 16:57:39.313762 acl_anthology_py-0.2.0/acl_anthology/utils/latex.py
+-rw-r--r--   0        0        0     2528 2023-08-07 13:45:11.703131 acl_anthology_py-0.2.0/acl_anthology/utils/logging.py
+-rw-r--r--   0        0        0     1078 2023-07-19 16:57:39.314762 acl_anthology_py-0.2.0/acl_anthology/utils/text.py
+-rw-r--r--   0        0        0     1927 2023-07-24 11:40:13.677609 acl_anthology_py-0.2.0/acl_anthology/utils/xml.py
+-rw-r--r--   0        0        0     1996 2023-08-08 12:48:15.139076 acl_anthology_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5426 1970-01-01 00:00:00.000000 acl_anthology_py-0.2.0/PKG-INFO
```

### Comparing `acl_anthology_py-0.1.0/LICENSE` & `acl_anthology_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acl_anthology_py-0.1.0/LICENSE.header` & `acl_anthology_py-0.2.0/LICENSE.header`

 * *Files identical despite different names*

### Comparing `acl_anthology_py-0.1.0/acl_anthology/__init__.py` & `acl_anthology_py-0.2.0/acl_anthology/text/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,9 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# ruff: noqa: F401
-from .anthology import Anthology
+from .markuptext import MarkupText
+from .texmath import TexMath
+
+
+__all__ = ["MarkupText", "TexMath"]
```

### Comparing `acl_anthology_py-0.1.0/acl_anthology/anthology.py` & `acl_anthology_py-0.2.0/acl_anthology/collections/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,22 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from pathlib import Path
-from .papers import PaperIndex
+from .index import CollectionIndex
+from .collection import Collection
+from .volume import Volume, VolumeType
+from .paper import Paper
 
-
-class Anthology:
-    def __init__(self, datadir):
-        if not Path(datadir).is_dir():
-            raise ValueError(f"Not a directory: {datadir}")  # TODO exception type
-
-        self._datadir = datadir
-        self.papers = PaperIndex(self)
-
-    @property
-    def datadir(self):
-        return self._datadir
+__all__ = ["CollectionIndex", "Collection", "Volume", "VolumeType", "Paper"]
```

### Comparing `acl_anthology_py-0.1.0/acl_anthology/logging.py` & `acl_anthology_py-0.2.0/acl_anthology/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,16 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import logging
-from rich.logging import RichHandler
+"""Constants used within the library."""
 
-FORMAT = "%(message)s"
-logging.basicConfig(
-    level="NOTSET", format=FORMAT, datefmt="[%X]", handlers=[RichHandler()]
-)
+from datetime import date
 
-log = logging.getLogger("acl-anthology")
+UNKNOWN_INGEST_DATE = date(1900, 1, 1)
+"""Default ingestion date."""
```

### Comparing `acl_anthology_py-0.1.0/acl_anthology/utils.py` & `acl_anthology_py-0.2.0/acl_anthology/utils/ids.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,32 +8,54 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional, Tuple
+"""Functions for manipulating Anthology IDs."""
 
+from typing import Optional
 
-def build_anthology_id(
-    collection_id: str, volume_id: str, paper_id: Optional[str] = None
+
+AnthologyID = str | tuple[str, Optional[str], Optional[str]]
+"""Any type that can be parsed into an Anthology ID."""
+
+
+def build_id(
+    collection_id: str, volume_id: Optional[str] = None, paper_id: Optional[str] = None
 ) -> str:
     """
-    Transforms collection id, volume id, and paper id to a width-padded
-    Anthology ID. e.g., ('P18', '1', '1') -> P18-1001.
+    Transforms collection ID, volume ID, and paper ID to a width-padded
+    Anthology ID.
+
+    Parameters:
+        collection_id: A collection ID, e.g. "P18".
+        volume_id: A volume ID, e.g. "1".
+        paper_id: A paper ID, e.g. "42".
+
+    Returns:
+        The full Anthology ID.
+
+    Examples:
+        >>> build_id("P18", "1", "1")
+        P18-1001
+        >>> build_id("2022.acl", "long", "42")
+        2022.acl-long.42
+
+    Warning:
+        Does not perform any kind of input validation.
     """
-    if collection_id[0].isdigit():
+    if volume_id is None:
+        return collection_id
+    elif collection_id[0].isdigit():
         if paper_id is not None:
             return f"{collection_id}-{volume_id}.{paper_id}"
-        elif volume_id is not None:
-            return f"{collection_id}-{volume_id}"
         else:
-            return collection_id
-
+            return f"{collection_id}-{volume_id}"
     else:  # pre-2020 IDs
         if (
             collection_id[0] == "W"
             or collection_id == "C69"
             or (collection_id == "D19" and int(volume_id) >= 5)
         ):
             anthology_id = f"{collection_id}-{int(volume_id):02d}"
@@ -43,50 +65,72 @@
             anthology_id = f"{collection_id}-{int(volume_id):01d}"
             if paper_id is not None:
                 anthology_id += f"{int(paper_id):03d}"
 
         return anthology_id
 
 
-def deconstruct_anthology_id(anthology_id: str) -> Tuple[str, str, str]:
+def parse_id(anthology_id: AnthologyID) -> tuple[str, Optional[str], Optional[str]]:
     """
-    Parses an Anthology ID into its constituent collection id, volume id, and paper id
-    parts. e.g,
-
-        P18-1007 -> ('P18', '1',  '7')
-        W18-6310 -> ('W18', '63', '10')
-        D19-1001 -> ('D19', '1',  '1')
-        D19-5702 -> ('D19', '57', '2')
-        2022.acl-main.1 -> ('2022.acl', 'main', '1')
-
-    Also works with volumes:
-
-        P18-1 -> ('P18', '1', None)
-        W18-63 -> ('W18', '63', None)
+    Parses an Anthology ID into its constituent collection ID, volume ID, and paper ID
+    parts.
 
-    And even with just collections:
+    Parameters:
+        anthology_id: The Anthology ID to parse.
 
-        P18 -> ('P18', None, None)
+    Returns:
+        The parsed collection ID, volume ID, and paper ID.
 
-    For Anthology IDs prior to 2020, the volume ID is the first digit after the hyphen, except
-    for the following situations, where it is the first two digits:
-
-    - All collections starting with 'W'
-    - The collection "C69"
-    - All collections in "D19" where the first digit is >= 5
+    Examples:
+        >>> parse_id("P18-1007")
+        ('P18', '1',  '7')
+        >>> parse_id("W18-6310")
+        ('W18', '63', '10')
+        >>> parse_id("D19-1001")
+        ('D19', '1',  '1')
+        >>> parse_id("D19-5702")
+        ('D19', '57', '2')
+        >>> parse_id("2022.acl-main.1")
+        ('2022.acl', 'main', '1')
+
+        Also works with volumes:
+
+        >>> parse_id("P18-1")
+        ('P18', '1', None)
+        >>> parse_id("W18-63")
+        ('W18', '63', None)
+
+        And even with just collections:
+
+        >>> parse_id("P18")
+        ('P18', None, None)
+
+    Warning:
+        Does not perform any kind of input validation.
+
+    Note:
+        For Anthology IDs prior to 2020, the volume ID is the first digit after the hyphen, except
+        for the following situations, where it is the first two digits:
+
+        - All collections starting with 'W'
+        - The collection "C69"
+        - All collections in "D19" where the first digit is >= 5
     """
 
+    if isinstance(anthology_id, tuple):
+        return anthology_id
+
     if "-" not in anthology_id:
         return (anthology_id, None, None)
 
     collection_id, rest = anthology_id.split("-")
     if collection_id[0].isdigit():
         # post-2020 IDs
         if "." in rest:
-            return (collection_id, *(rest.split(".")))
+            return (collection_id, *(rest.split(".")))  # type: ignore
         else:
             return (collection_id, rest, None)
     else:
         # pre-2020 IDs
         if len(rest) < 4:
             # probably volume-only identifier
             return (collection_id, rest.lstrip("0"), None)
```

### Comparing `acl_anthology_py-0.1.0/pyproject.toml` & `acl_anthology_py-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,77 @@
 [tool.black]
 line-length = 90
-target-version = ['py311']
+target-version = ['py310', 'py311']
 skip-string-normalization = false
 
+[tool.mypy]
+strict = true
+
+[[tool.mypy.overrides]]
+module = 'TexSoup.*'
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = 'latexcodec.*'
+ignore_missing_imports = true
+
 [tool.ruff]
 ignore = ['E501']  # "Line too long" is black's job
-target-version = 'py311'
+target-version = 'py310'
 
 [tool.poetry]
 name = "acl-anthology-py"
 packages = [
     { include = "acl_anthology" },
 ]
-version = "0.1.0"
+version = "0.2.0"
 description = "A library for accessing the ACL Anthology"
 authors = ["Marcel Bollmann <marcel@bollmann.me>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/mbollmann/acl-anthology-py"
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10,!=3.11.0"
 docopt = "^0.6.2"
 latexcodec = "^2.0.1"
 lxml = "^4.9.2"
 PyYAML = "^6.0"
 app-paths = "^0.0.7"
 diskcache = "^5.6.1"
 rich = "^13.3.5"
+attrs = "^23.1.0"
+texsoup = ">=0.3.1,<0.4.0"
+omegaconf = "^2.3.0"
+python-slugify = {extras = ["unidecode"], version = "^8.0.1"}
+scipy = "^1.6.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.269"
 pre-commit = "^3.3.2"
 richbench = "^1.0.3"
+mkdocs = "^1.4.3"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-material = "^9.1.15"
+mypy = "^1.3.0"
+lxml-stubs = "^0.4.0"
+types-python-slugify = "^8.0.0.3"
+types-pyyaml = "^6.0.12.11"
+scalene = { git = "https://github.com/plasma-umass/scalene.git" }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

