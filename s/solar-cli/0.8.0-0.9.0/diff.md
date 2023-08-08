# Comparing `tmp/solar_cli-0.8.0.tar.gz` & `tmp/solar_cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_cli-0.8.0.tar", max compression
+gzip compressed data, was "solar_cli-0.9.0.tar", max compression
```

## Comparing `solar_cli-0.8.0.tar` & `solar_cli-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3121 2023-08-08 08:54:08.454260 solar_cli-0.8.0/README.md
--rw-r--r--   0        0        0      612 2023-08-08 09:54:59.667094 solar_cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       51 2023-08-08 09:33:57.514927 solar_cli-0.8.0/solar/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 08:54:08.454260 solar_cli-0.8.0/solar/api/__init__.py
--rw-r--r--   0        0        0     6665 2023-08-08 09:54:55.247040 solar_cli-0.8.0/solar/api/base.py
--rw-r--r--   0        0        0     7900 2023-08-08 08:54:08.454260 solar_cli-0.8.0/solar/api/export.py
--rw-r--r--   0        0        0     7983 2023-08-08 09:49:28.310417 solar_cli-0.8.0/solar/api/import_.py
--rw-r--r--   0        0        0     6771 2023-08-08 09:54:24.582780 solar_cli-0.8.0/solar/cli.py
--rw-r--r--   0        0        0       98 2023-08-08 08:54:08.454260 solar_cli-0.8.0/solar/cmd/__init__.py
--rw-r--r--   0        0        0     2011 2023-08-08 08:58:36.034207 solar_cli-0.8.0/solar/cmd/export.py
--rw-r--r--   0        0        0     1665 2023-08-08 08:58:10.424206 solar_cli-0.8.0/solar/cmd/import_.py
--rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.8.0/solar/types/__init__.py
--rw-r--r--   0        0        0      481 2023-08-08 08:54:08.464260 solar_cli-0.8.0/solar/types/analysis.py
--rw-r--r--   0        0        0      141 2023-08-08 08:54:08.464260 solar_cli-0.8.0/solar/types/base.py
--rw-r--r--   0        0        0     1278 2023-08-08 08:54:08.464260 solar_cli-0.8.0/solar/types/cluster_status.py
--rw-r--r--   0        0        0      331 2023-08-08 08:54:08.464260 solar_cli-0.8.0/solar/types/config_files.py
--rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.8.0/solar/utils.py
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 solar_cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     3121 2023-08-08 08:54:08.454260 solar_cli-0.9.0/README.md
+-rw-r--r--   0        0        0      612 2023-08-08 10:04:42.992251 solar_cli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-08-08 09:33:57.514927 solar_cli-0.9.0/solar/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:54:08.454260 solar_cli-0.9.0/solar/api/__init__.py
+-rw-r--r--   0        0        0     7022 2023-08-08 10:04:39.052240 solar_cli-0.9.0/solar/api/base.py
+-rw-r--r--   0        0        0     7900 2023-08-08 08:54:08.454260 solar_cli-0.9.0/solar/api/export.py
+-rw-r--r--   0        0        0     7983 2023-08-08 09:49:28.310417 solar_cli-0.9.0/solar/api/import_.py
+-rw-r--r--   0        0        0     7347 2023-08-08 10:04:14.910993 solar_cli-0.9.0/solar/cli.py
+-rw-r--r--   0        0        0       98 2023-08-08 08:54:08.454260 solar_cli-0.9.0/solar/cmd/__init__.py
+-rw-r--r--   0        0        0     2011 2023-08-08 08:58:36.034207 solar_cli-0.9.0/solar/cmd/export.py
+-rw-r--r--   0        0        0     1665 2023-08-08 08:58:10.424206 solar_cli-0.9.0/solar/cmd/import_.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.9.0/solar/types/__init__.py
+-rw-r--r--   0        0        0      481 2023-08-08 08:54:08.464260 solar_cli-0.9.0/solar/types/analysis.py
+-rw-r--r--   0        0        0      141 2023-08-08 08:54:08.464260 solar_cli-0.9.0/solar/types/base.py
+-rw-r--r--   0        0        0     1278 2023-08-08 08:54:08.464260 solar_cli-0.9.0/solar/types/cluster_status.py
+-rw-r--r--   0        0        0      331 2023-08-08 08:54:08.464260 solar_cli-0.9.0/solar/types/config_files.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.9.0/solar/utils.py
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 solar_cli-0.9.0/PKG-INFO
```

### Comparing `solar_cli-0.8.0/README.md` & `solar_cli-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `solar_cli-0.8.0/pyproject.toml` & `solar_cli-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solar-cli"
-version = "0.8.0"
+version = "0.9.0"
 description = "CLI app for Solr"
 authors = ["Andrey S. <andrewsapw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "solar" },
 ]
```

### Comparing `solar_cli-0.8.0/solar/api/base.py` & `solar_cli-0.9.0/solar/api/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,7 +200,17 @@
         url = "/solr/admin/collections?action=LIST&wt=json"
         resp = await self.api_request(path=url)
         if resp is None:
             raise ValueError("Error fetching collections")
 
         data = json.loads(resp)
         return data["collections"]
+
+    @property
+    async def configs(self):
+        url = "/solr/admin/zookeeper?detail=false&path=/configs/&wt=json"
+        resp = await self.api_request(path=url)
+        if resp is None:
+            raise ValueError("Error fetching collections")
+
+        data = json.loads(resp)
+        return [i["text"] for i in data["tree"][0]["children"]]
```

### Comparing `solar_cli-0.8.0/solar/api/export.py` & `solar_cli-0.9.0/solar/api/export.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.8.0/solar/api/import_.py` & `solar_cli-0.9.0/solar/api/import_.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.8.0/solar/cli.py` & `solar_cli-0.9.0/solar/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,9 +220,32 @@
         print(result)
     except Exception as e:
         print(f"[red]{e}")
         exit(1)
     finally:
         await engine.close_client()
 
+@cli.command(name="configs")
+@click.pass_context
+@coro
+async def show_configs(ctx):
+    """Remove config from Solr"""
+    ctx.ensure_object(dict)
+
+    engine = ApiEngine(
+        base_url=ctx.obj["url"],
+        collection=ctx.obj["collection"],
+        username=ctx.obj["username"],
+        password=ctx.obj["password"],
+    )
+    try:
+        await engine.build_client()
+        result = await engine.configs
+        print(result)
+    except Exception as e:
+        print(f"[red]{e}")
+        exit(1)
+    finally:
+        await engine.close_client()
+
 if __name__ == "__main__":
     cli()
```

### Comparing `solar_cli-0.8.0/solar/cmd/export.py` & `solar_cli-0.9.0/solar/cmd/export.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.8.0/solar/cmd/import_.py` & `solar_cli-0.9.0/solar/cmd/import_.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.8.0/solar/types/cluster_status.py` & `solar_cli-0.9.0/solar/types/cluster_status.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.8.0/PKG-INFO` & `solar_cli-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI app for Solr
 License: MIT
 Author: Andrey S.
 Author-email: andrewsapw@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

