# Comparing `tmp/solar-cli-0.1.0.tar.gz` & `tmp/solar_cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar-cli-0.1.0.tar", max compression
+gzip compressed data, was "solar_cli-0.6.0.tar", max compression
```

## Comparing `solar-cli-0.1.0.tar` & `solar_cli-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      612 2023-03-17 08:41:11.686924 solar-cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3059 2023-03-17 08:18:01.758399 solar-cli-0.1.0/README.md
--rw-r--r--   0        0        0       36 2023-03-17 08:24:01.242760 solar-cli-0.1.0/solar/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 08:27:02.874918 solar-cli-0.1.0/solar/api/__init__.py
--rw-r--r--   0        0        0     5174 2023-03-16 09:40:39.337530 solar-cli-0.1.0/solar/api/base.py
--rw-r--r--   0        0        0     7793 2023-03-17 08:27:37.025501 solar-cli-0.1.0/solar/api/export.py
--rw-r--r--   0        0        0     7850 2023-03-17 08:27:43.639505 solar-cli-0.1.0/solar/api/import_.py
--rw-r--r--   0        0        0     5224 2023-03-17 08:27:29.879099 solar-cli-0.1.0/solar/cli.py
--rw-r--r--   0        0        0       98 2023-03-17 08:29:25.449458 solar-cli-0.1.0/solar/cmd/__init__.py
--rw-r--r--   0        0        0     1810 2023-03-17 08:29:23.627858 solar-cli-0.1.0/solar/cmd/export.py
--rw-r--r--   0        0        0     1585 2023-03-17 08:29:23.629855 solar-cli-0.1.0/solar/cmd/import_.py
--rw-r--r--   0        0        0        0 2023-03-16 08:04:17.380230 solar-cli-0.1.0/solar/types/__init__.py
--rw-r--r--   0        0        0      141 2023-03-17 08:18:01.761026 solar-cli-0.1.0/solar/types/base.py
--rw-r--r--   0        0        0     1278 2023-03-17 08:18:01.761069 solar-cli-0.1.0/solar/types/cluster_status.py
--rw-r--r--   0        0        0      331 2023-03-17 08:18:01.761570 solar-cli-0.1.0/solar/types/config_files.py
--rw-r--r--   0        0        0        0 2023-03-16 08:00:30.726867 solar-cli-0.1.0/solar/types.py
--rw-r--r--   0        0        0        0 2023-03-15 08:59:40.030560 solar-cli-0.1.0/solar/utils.py
--rw-r--r--   0        0        0     3937 1970-01-01 00:00:00.000000 solar-cli-0.1.0/setup.py
--rw-r--r--   0        0        0     3685 1970-01-01 00:00:00.000000 solar-cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3121 2023-08-08 08:54:08.454260 solar_cli-0.6.0/README.md
+-rw-r--r--   0        0        0      612 2023-08-08 08:54:08.454260 solar_cli-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-08-08 08:54:08.454260 solar_cli-0.6.0/solar/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:54:08.454260 solar_cli-0.6.0/solar/api/__init__.py
+-rw-r--r--   0        0        0     6347 2023-08-08 08:58:23.614207 solar_cli-0.6.0/solar/api/base.py
+-rw-r--r--   0        0        0     7900 2023-08-08 08:54:08.454260 solar_cli-0.6.0/solar/api/export.py
+-rw-r--r--   0        0        0     7879 2023-08-08 08:57:33.484230 solar_cli-0.6.0/solar/api/import_.py
+-rw-r--r--   0        0        0     6152 2023-08-08 08:57:03.184229 solar_cli-0.6.0/solar/cli.py
+-rw-r--r--   0        0        0       98 2023-08-08 08:54:08.454260 solar_cli-0.6.0/solar/cmd/__init__.py
+-rw-r--r--   0        0        0     2011 2023-08-08 08:58:36.034207 solar_cli-0.6.0/solar/cmd/export.py
+-rw-r--r--   0        0        0     1665 2023-08-08 08:58:10.424206 solar_cli-0.6.0/solar/cmd/import_.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/__init__.py
+-rw-r--r--   0        0        0      481 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/analysis.py
+-rw-r--r--   0        0        0      141 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/base.py
+-rw-r--r--   0        0        0     1278 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/cluster_status.py
+-rw-r--r--   0        0        0      331 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/config_files.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/utils.py
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 solar_cli-0.6.0/PKG-INFO
```

### Comparing `solar-cli-0.1.0/pyproject.toml` & `solar_cli-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solar-cli"
-version = "0.1.0"
+version = "0.6.0"
 description = "CLI app for Solr"
 authors = ["Andrey S. <andrewsapw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "solar" },
 ]
```

### Comparing `solar-cli-0.1.0/README.md` & `solar_cli-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 - Import / Export data
 - Import / Export configs
 - Re-index Collection (WIP)
 
 
 # Usage
 
+> Python version >=3.8 required
+
+`pip install solar-cli`
+
 # Export
 
 ## Export data
 
 This command will save docs from `<collection>` to local folder `./data`:
 ```sh
 solar -c "<collection>" "https://<username>:<password>@localhost:8333" export ./data
@@ -36,20 +40,20 @@
 
 # Import
 
 ## Import data
 
 Later, we can import previously exported data with `import` command, and `./data/<collection>.json` as source file:
 ```sh
-solar "https://<username>:<password>@localhost:8333" export ./data/<collection>.json
+solar "https://<username>:<password>@localhost:8333" import ./data/<collection>.json
 ```
 
 We do not have to specify collection name, source `.json` already have collection name. However, if we want to import data as collection with different name, we can set this with `-c` flag:
 ```sh
-solar -c "<new collection name>" "https://<username>:<password>@localhost:8333" export ./data/<collection>.json
+solar -c "<new collection name>" "https://<username>:<password>@localhost:8333" import ./data/<collection>.json
 ```
 
 ## Import config
 
 Solar can help you import configsets to your Solr instance:
 ```sh
 solar -c "https://<username>:<password>@localhost:8333" import-config <config folder path>
```

### Comparing `solar-cli-0.1.0/solar/api/base.py` & `solar_cli-0.6.0/solar/api/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import logging
 from typing import List, Optional
 
 import aiohttp
 import orjson
+from more_itertools import chunked
 
+from solar.types.analysis import AnalysisModel
 from solar.types.cluster_status import ClusterStatus
 
 # requests.packages.urllib3.disable_warnings()  # type: ignore
 logger = logging.getLogger("root")
 
 
 class ApiEngine:
@@ -118,15 +120,15 @@
                 logger.error(f"{method} - {resp.url} - {text}")
                 return None
 
             try:
                 return await resp.text(encoding="UTF-8")
             except UnicodeDecodeError as e:
                 print("Can't decode answer :( {e}")
-                return None
+                exit(1)
 
     async def remove_collection(self, collection_name: str):
         url = f"/solr/admin/collections?action=DELETE&name={collection_name}"
         await self.api_request(path=url)
 
     async def reload_collection(self, collection_name: str):
         url = f"/solr/admin/collections?action=RELOAD&name={collection_name}"
@@ -155,7 +157,40 @@
     async def remove_alias(self, alias_name: str):
         url = "/solr/admin/collections?action=DELETEALIAS"
         params = dict(name=alias_name)
 
         resp = await self.api_request(path=url, params=params)
         if resp is None:
             raise ValueError(f"Error removing alias {alias_name}")
+
+    async def analyzer_step(self, field: str, analyzer: str, text: str):
+        url = f"/solr/{self.collection}/analysis/field"
+        params = {
+            "analysis.fieldname": field,
+            "analysis.fieldvalue": text,
+            "analysis.showmatch": "false",
+            "verbose_output": 0,
+        }
+        resp = await self.api_request(path=url, params=params)
+        if resp is None:
+            raise ValueError("Error fetching analysis result")
+
+        data = json.loads(resp)
+        analysis = AnalysisModel(**data)
+
+        parsed_tokens = []
+        for step_name, result in chunked(
+            analysis.analysis.field_names.content.index, 2
+        ):
+            if analyzer not in step_name:
+                continue
+
+            if isinstance(result, str):
+                analyzer_result = result
+                return analyzer_result
+
+            for i in result:
+                token = i["text"]
+                parsed_tokens.append(token)
+
+        analyzer_result = " ".join(parsed_tokens)
+        return analyzer_result
```

### Comparing `solar-cli-0.1.0/solar/api/export.py` & `solar_cli-0.6.0/solar/api/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         return doc
 
     async def _export_to_path(
         self,
         query: str,
         path: Union[str, pathlib.Path],
         nested: bool,
-        batch_size: int = 100,
+        batch_size: int = 10,
         name: Optional[str] = None,
     ) -> Optional[pathlib.Path]:
         """Export documents to .json file in `path`
 
         Args:
             query (str): `q` parameter to fetch docs from Solr
             path (str): path to save result `.json` file
@@ -127,29 +127,31 @@
 
     async def export_data(
         self,
         path: Union[str, pathlib.Path],
         query: str = "*:*",
         nested: bool = False,
         name: Optional[str] = None,
+        batch_size: Optional[int] = 50,
     ) -> Optional[pathlib.Path]:
         """Export Solr collection to `path`
 
         Args:
             path (str): path to save result `.json` file
             query (str, optional): `q` parameter to fetch docs from Solr
                 Defaults to "*:*".
 
         Returns:
             Optional[pathlib.Path]: result `.json` path
         """
         print(f"Export nested documents: {nested}")
+        print(f"Batch size: {batch_size}")
 
         filepath = await self._export_to_path(
-            path=path, query=query, nested=nested, name=name
+            path=path, query=query, nested=nested, name=name, batch_size=batch_size
         )
 
         return filepath
 
     async def export_config(
         self, path: Union[str, pathlib.Path], collection_name: str
     ) -> Optional[pathlib.Path]:
```

### Comparing `solar-cli-0.1.0/solar/api/import_.py` & `solar_cli-0.6.0/solar/api/import_.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,15 @@
             for batch_docs in chunked(upload_docs, batch_size):
                 try:
                     await self._post_documents(
                         docs=batch_docs, collection_name=collection_name
                     )
                 except Exception:
                     print("[red]Ошибка :)")
+                    exit(1)
 
                 progress.update(task, advance=batch_size)
 
     async def _remove_config(self, name: str):
         url = f"/api/cluster/configs/{name}?omitHeader=true"
         r = await self.api_request(method="DELETE", path=url)
         if r is None:
```

### Comparing `solar-cli-0.1.0/solar/cli.py` & `solar_cli-0.6.0/solar/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
 import datetime
+import os
 import pathlib
 import urllib.parse
 from functools import wraps
 
 import click
 from rich import print
 
+from solar.api.base import ApiEngine
 from solar.api.export import Exporter
 from solar.api.import_ import Importer
 from solar.types.cluster_status import Collection
 
 
 def coro(f):
     @wraps(f)
@@ -26,15 +28,16 @@
 @click.option("-c", "--collection", default=None)
 @click.pass_context
 def cli(ctx, query: str, collection: str, url: str):
     """Solr CLI"""
     url_parsed = urllib.parse.urlparse(url)
     if url_parsed.scheme not in ("http", "https"):
         print(f"[red]Unknown scheme {url_parsed.scheme}")
-        return
+        exit(1)
+        
 
     username = url_parsed.username
     password = url_parsed.password
 
     url_str = f"{url_parsed.scheme}://{url_parsed.hostname}:{url_parsed.port}{url_parsed.path}"
 
     ctx.ensure_object(dict)
@@ -55,20 +58,22 @@
     importer = Importer(
         base_url=ctx.obj["url"],
         collection=ctx.obj["collection"],
         username=ctx.obj["username"],
         password=ctx.obj["password"],
     )
     try:
-        confirm = input(f"Вы точно хотите удалить конфиг {name}").lower() == "y"
+        confirm = input(f"You sure you want to delete config {name}?").lower() == "y"
         if not confirm:
             return
 
         await importer.build_client()
         await importer._remove_config(name=name)
+    except Exception:
+        exit(1)
     finally:
         await importer.close_client()
 
 
 @cli.command(name="reindex")
 @click.option("--cpath", default=None, help="New config path")
 @click.option("--cname", default=None, help="New config name")
@@ -79,15 +84,15 @@
     """Reindex collection"""
     work_dir = pathlib.Path(directory)
     if not work_dir.exists():
         work_dir.mkdir()
 
     if ctx.obj["collection"] is None:
         print("[bold red]Connection parament have to specified")
-        return
+        exit(1)
 
     collection_name = ctx.obj["collection"].strip()
 
     ctx.ensure_object(dict)
     importer = Importer(
         base_url=ctx.obj["url"],
         collection=ctx.obj["collection"],
@@ -153,15 +158,46 @@
             collection_name=collection_name, config_name=new_config_name
         )
         print("[green]Success")
 
         print(f"Importing data to collection [bold]{collection_name}")
         await importer.import_data(path=tmp_data_path, collection=collection_name)
         print("[green]Success")
-
+    except Exception:
+        exit(1)
     finally:
         await importer.close_client()
         await exporter.close_client()
 
 
+@cli.command(name="analyzer-step")
+@click.argument("field")
+@click.argument("analyzer")
+@click.argument("text")
+@click.pass_context
+@coro
+async def analyzer_step(ctx, field, analyzer, text):
+    """Remove config from Solr"""
+    ctx.ensure_object(dict)
+
+    if ctx.obj["collection"] is None:
+        print("[red]Missing --collection flag")
+        return
+
+    engine = ApiEngine(
+        base_url=ctx.obj["url"],
+        collection=ctx.obj["collection"],
+        username=ctx.obj["username"],
+        password=ctx.obj["password"],
+    )
+    try:
+        await engine.build_client()
+        result = await engine.analyzer_step(field=field, analyzer=analyzer, text=text)
+        print(result)
+    except Exception:
+        exit(1)
+    finally:
+        await engine.close_client()
+
+
 if __name__ == "__main__":
     cli()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `solar-cli-0.1.0/solar/cmd/export.py` & `solar_cli-0.6.0/solar/cmd/export.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,23 @@
 @click.option(
     "--nested",
     is_flag=True,
     show_default=True,
     default=False,
     help="Export nested documents. Default: False",
 )
+@click.option(
+    "--batch",
+    type=int,
+    default=50,
+    help="Batch size",
+)
 @click.pass_context
 @coro
-async def export_data(ctx, directory, nested: bool):
+async def export_data(ctx, directory, nested: bool, batch: int):
     """Export data from Solr"""
     ctx.ensure_object(dict)
     if ctx.obj["collection"] is None:
         print("[bold red]Параметр collection должен быть задан")
         return
 
     exporter = Exporter(
@@ -28,16 +34,18 @@
         collection=ctx.obj["collection"],
         username=ctx.obj["username"],
         password=ctx.obj["password"],
     )
     try:
         await exporter.build_client()
         await exporter.export_data(
-            path=directory, query=ctx.obj["query"], nested=nested
+            path=directory, query=ctx.obj["query"], nested=nested, batch_size=batch
         )
+    except Exception:
+        exit(1)
     finally:
         await exporter.close_client()
 
 
 @cli.command(name="export-config")
 @click.argument("directory")
 @click.pass_context
@@ -58,9 +66,11 @@
     )
     try:
         await exporter.build_client()
         await exporter.export_config(
             path=directory, collection_name=ctx.obj["collection"]
         )
         print("[green]Done!")
+    except Exception:
+        exit(1)
     finally:
         await exporter.close_client()
```

### Comparing `solar-cli-0.1.0/solar/cmd/import_.py` & `solar_cli-0.6.0/solar/cmd/import_.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         collection=ctx.obj["collection"],
         username=ctx.obj["username"],
         password=ctx.obj["password"],
     )
     try:
         await importer.build_client()
         await importer.import_data(path=filepath, batch_size=batch)
+    except Exception:
+        exit(1)
     finally:
         await importer.close_client()
 
 
 @cli.command(name="import-config")
 @click.argument("directory")
 @click.option(
@@ -47,9 +49,11 @@
         password=ctx.obj["password"],
     )
     try:
         await importer.build_client()
         await importer.import_configs(
             configs_path=directory, overwrite=overwrite, name=name
         )
+    except Exception:
+        exit(1)
     finally:
         await importer.close_client()
```

### Comparing `solar-cli-0.1.0/solar/types/cluster_status.py` & `solar_cli-0.6.0/solar/types/cluster_status.py`

 * *Files identical despite different names*

### Comparing `solar-cli-0.1.0/setup.py` & `solar_cli-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,112 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: solar-cli
+Version: 0.6.0
+Summary: CLI app for Solr
+License: MIT
+Author: Andrey S.
+Author-email: andrewsapw@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
+Requires-Dist: orjson (>=3.8.7,<4.0.0)
+Requires-Dist: pydantic (>=1.10.6,<2.0.0)
+Requires-Dist: rich (>=13.3.2,<14.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['solar', 'solar.api', 'solar.cmd', 'solar.types']
+# Solar
 
-package_data = \
-{'': ['*']}
+This CLI tool provides help with some routine Solr operations:
+- Import / Export data
+- Import / Export configs
+- Re-index Collection (WIP)
 
-install_requires = \
-['aiohttp>=3.8.4,<4.0.0',
- 'click>=8.1.3,<9.0.0',
- 'more-itertools>=9.1.0,<10.0.0',
- 'orjson>=3.8.7,<4.0.0',
- 'pydantic>=1.10.6,<2.0.0',
- 'rich>=13.3.2,<14.0.0']
-
-entry_points = \
-{'console_scripts': ['solar = solar.cli:cli']}
-
-setup_kwargs = {
-    'name': 'solar-cli',
-    'version': '0.1.0',
-    'description': 'CLI app for Solr',
-    'long_description': '# Solar\n\nThis CLI tool provides help with some routine Solr operations:\n- Import / Export data\n- Import / Export configs\n- Re-index Collection (WIP)\n\n\n# Usage\n\n# Export\n\n## Export data\n\nThis command will save docs from `<collection>` to local folder `./data`:\n```sh\nsolar -c "<collection>" "https://<username>:<password>@localhost:8333" export ./data\n```\n\n### Export nested documents\nSolr can handle nested documents. To see nested structure of collection usually we add `fl="*, [child]"` to our query params. Solar can handle exporting nested documents by adding `--nested` flag:\n```sh\nsolar -c "<collection>" "https://<username>:<password>@localhost:8333" export --nested ./data\n```\n\n\n\n## Export config\n\nIf we want to save collection config, we can user `export-config` command:\n\n```sh\nsolar -c "<collection>" "https://<username>:<password>@localhost:8333" export-config ./configs\n```\nThis will all config files to local folder `./configs`\n\n# Import\n\n## Import data\n\nLater, we can import previously exported data with `import` command, and `./data/<collection>.json` as source file:\n```sh\nsolar "https://<username>:<password>@localhost:8333" export ./data/<collection>.json\n```\n\nWe do not have to specify collection name, source `.json` already have collection name. However, if we want to import data as collection with different name, we can set this with `-c` flag:\n```sh\nsolar -c "<new collection name>" "https://<username>:<password>@localhost:8333" export ./data/<collection>.json\n```\n\n## Import config\n\nSolar can help you import configsets to your Solr instance:\n```sh\nsolar -c "https://<username>:<password>@localhost:8333" import-config <config folder path>\n```\n\nThis command will read files from provide config path, zip them, and send to Solr. By default, created config name will be equal to config folder name. For example, if we import config from `./configs/products`, Solar will create config named `products`.\n\nIf we want to override default name, we can use `--name` flag:\n\n```sh\nsolar -c "https://<username>:<password>@localhost:8333" import-config --name "product-v2" <config folder path>\n```\n\nThis will create config `product-v2`.\n\nAlso, we can overwrite existing config with `--overwrite` flag\n> This flag will add `cleanup=true` and `overwrite=true` params to request for creating config. However it is recommended to create config with the *new* name, because in some cases, Solr caches fields types, and some changes of new config will not be applied. Goog practice is version control your configs and name them with version identifier (commit hash, for example)\n> Using this flag also requires that no collections is linked to this config\n\n```sh\nsolar -c "https://<username>:<password>@localhost:8333" import-config --overwrite <config folder path>\n```\n\n# Other\n\n## Remove config\n\nConfig `<config name>` can be removed from Solr with this command:\n\n```sh\nsolar -c "https://<username>:<password>@localhost:8333" remove-config "<config name>"\n\n```\n',
-    'author': 'Andrey S.',
-    'author_email': 'andrewsapw@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
 
+# Usage
+
+> Python version >=3.8 required
+
+`pip install solar-cli`
+
+# Export
+
+## Export data
+
+This command will save docs from `<collection>` to local folder `./data`:
+```sh
+solar -c "<collection>" "https://<username>:<password>@localhost:8333" export ./data
+```
+
+### Export nested documents
+Solr can handle nested documents. To see nested structure of collection usually we add `fl="*, [child]"` to our query params. Solar can handle exporting nested documents by adding `--nested` flag:
+```sh
+solar -c "<collection>" "https://<username>:<password>@localhost:8333" export --nested ./data
+```
+
+
+
+## Export config
+
+If we want to save collection config, we can user `export-config` command:
+
+```sh
+solar -c "<collection>" "https://<username>:<password>@localhost:8333" export-config ./configs
+```
+This will all config files to local folder `./configs`
+
+# Import
+
+## Import data
+
+Later, we can import previously exported data with `import` command, and `./data/<collection>.json` as source file:
+```sh
+solar "https://<username>:<password>@localhost:8333" import ./data/<collection>.json
+```
+
+We do not have to specify collection name, source `.json` already have collection name. However, if we want to import data as collection with different name, we can set this with `-c` flag:
+```sh
+solar -c "<new collection name>" "https://<username>:<password>@localhost:8333" import ./data/<collection>.json
+```
+
+## Import config
+
+Solar can help you import configsets to your Solr instance:
+```sh
+solar -c "https://<username>:<password>@localhost:8333" import-config <config folder path>
+```
+
+This command will read files from provide config path, zip them, and send to Solr. By default, created config name will be equal to config folder name. For example, if we import config from `./configs/products`, Solar will create config named `products`.
+
+If we want to override default name, we can use `--name` flag:
+
+```sh
+solar -c "https://<username>:<password>@localhost:8333" import-config --name "product-v2" <config folder path>
+```
+
+This will create config `product-v2`.
+
+Also, we can overwrite existing config with `--overwrite` flag
+> This flag will add `cleanup=true` and `overwrite=true` params to request for creating config. However it is recommended to create config with the *new* name, because in some cases, Solr caches fields types, and some changes of new config will not be applied. Goog practice is version control your configs and name them with version identifier (commit hash, for example)
+> Using this flag also requires that no collections is linked to this config
+
+```sh
+solar -c "https://<username>:<password>@localhost:8333" import-config --overwrite <config folder path>
+```
+
+# Other
+
+## Remove config
+
+Config `<config name>` can be removed from Solr with this command:
+
+```sh
+solar -c "https://<username>:<password>@localhost:8333" remove-config "<config name>"
+
+```
 
-setup(**setup_kwargs)
```

