# Comparing `tmp/naist-codehash-0.0.2.tar.gz` & `tmp/naist-codehash-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naist-codehash-0.0.2.tar", last modified: Tue Aug  8 17:18:32 2023, max compression
+gzip compressed data, was "naist-codehash-0.0.3.tar", last modified: Tue Aug  8 17:21:00 2023, max compression
```

## Comparing `naist-codehash-0.0.2.tar` & `naist-codehash-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 dora      (1000) dora      (1000)        0 2023-08-08 17:18:32.971598 naist-codehash-0.0.2/
--rwxrwxrwx   0 dora      (1000) dora      (1000)     1075 2023-08-08 07:06:34.000000 naist-codehash-0.0.2/LICENSE
--rwxrwxrwx   0 dora      (1000) dora      (1000)       28 2023-08-08 07:06:34.000000 naist-codehash-0.0.2/MANIFEST.in
--rwxrwxrwx   0 dora      (1000) dora      (1000)      324 2023-08-08 17:18:32.969596 naist-codehash-0.0.2/PKG-INFO
--rwxrwxrwx   0 dora      (1000) dora      (1000)      189 2023-08-08 07:26:17.000000 naist-codehash-0.0.2/README.md
-drwxrwxrwx   0 dora      (1000) dora      (1000)        0 2023-08-08 17:18:32.906595 naist-codehash-0.0.2/codehash/
--rwxrwxrwx   0 dora      (1000) dora      (1000)       31 2023-08-08 16:49:32.000000 naist-codehash-0.0.2/codehash/__init__.py
--rwxrwxrwx   0 dora      (1000) dora      (1000)     5780 2023-08-08 16:55:16.000000 naist-codehash-0.0.2/codehash/codehash.py
-drwxrwxrwx   0 dora      (1000) dora      (1000)        0 2023-08-08 17:18:32.955596 naist-codehash-0.0.2/naist_codehash.egg-info/
--rwxrwxrwx   0 dora      (1000) dora      (1000)      324 2023-08-08 17:18:32.000000 naist-codehash-0.0.2/naist_codehash.egg-info/PKG-INFO
--rwxrwxrwx   0 dora      (1000) dora      (1000)      232 2023-08-08 17:18:32.000000 naist-codehash-0.0.2/naist_codehash.egg-info/SOURCES.txt
--rwxrwxrwx   0 dora      (1000) dora      (1000)        1 2023-08-08 17:18:32.000000 naist-codehash-0.0.2/naist_codehash.egg-info/dependency_links.txt
--rwxrwxrwx   0 dora      (1000) dora      (1000)        9 2023-08-08 17:18:32.000000 naist-codehash-0.0.2/naist_codehash.egg-info/top_level.txt
--rwxrwxrwx   0 dora      (1000) dora      (1000)       38 2023-08-08 17:18:32.972597 naist-codehash-0.0.2/setup.cfg
--rwxrwxrwx   0 dora      (1000) dora      (1000)      438 2023-08-08 17:18:29.000000 naist-codehash-0.0.2/setup.py
+drwxrwxrwx   0 dora      (1000) dora      (1000)        0 2023-08-08 17:21:00.349958 naist-codehash-0.0.3/
+-rwxrwxrwx   0 dora      (1000) dora      (1000)     1075 2023-08-08 07:06:34.000000 naist-codehash-0.0.3/LICENSE
+-rwxrwxrwx   0 dora      (1000) dora      (1000)       28 2023-08-08 07:06:34.000000 naist-codehash-0.0.3/MANIFEST.in
+-rwxrwxrwx   0 dora      (1000) dora      (1000)      324 2023-08-08 17:21:00.347958 naist-codehash-0.0.3/PKG-INFO
+-rwxrwxrwx   0 dora      (1000) dora      (1000)      189 2023-08-08 07:26:17.000000 naist-codehash-0.0.3/README.md
+drwxrwxrwx   0 dora      (1000) dora      (1000)        0 2023-08-08 17:21:00.281405 naist-codehash-0.0.3/codehash/
+-rwxrwxrwx   0 dora      (1000) dora      (1000)       31 2023-08-08 16:49:32.000000 naist-codehash-0.0.3/codehash/__init__.py
+-rwxrwxrwx   0 dora      (1000) dora      (1000)     5761 2023-08-08 17:20:54.000000 naist-codehash-0.0.3/codehash/codehash.py
+drwxrwxrwx   0 dora      (1000) dora      (1000)        0 2023-08-08 17:21:00.331962 naist-codehash-0.0.3/naist_codehash.egg-info/
+-rwxrwxrwx   0 dora      (1000) dora      (1000)      324 2023-08-08 17:21:00.000000 naist-codehash-0.0.3/naist_codehash.egg-info/PKG-INFO
+-rwxrwxrwx   0 dora      (1000) dora      (1000)      232 2023-08-08 17:21:00.000000 naist-codehash-0.0.3/naist_codehash.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dora      (1000) dora      (1000)        1 2023-08-08 17:21:00.000000 naist-codehash-0.0.3/naist_codehash.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dora      (1000) dora      (1000)        9 2023-08-08 17:21:00.000000 naist-codehash-0.0.3/naist_codehash.egg-info/top_level.txt
+-rwxrwxrwx   0 dora      (1000) dora      (1000)       38 2023-08-08 17:21:00.349958 naist-codehash-0.0.3/setup.cfg
+-rwxrwxrwx   0 dora      (1000) dora      (1000)      438 2023-08-08 17:20:40.000000 naist-codehash-0.0.3/setup.py
```

### Comparing `naist-codehash-0.0.2/LICENSE` & `naist-codehash-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `naist-codehash-0.0.2/codehash/codehash.py` & `naist-codehash-0.0.3/codehash/codehash.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
             },
         ]
         for submit in cs:
             fname = "tmp/" + submit[self.ID_KEY] + ".py"
             with open(fname, "w") as f:
                 f.write(submit["code"])
             cmd.append(fname)
-        print(cmd)
         res = subprocess.run(
             cmd,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE)
         sout = res.stdout.decode("utf8")
         jsdata = json.loads(sout)
         shutil.rmtree("./tmp")
```

