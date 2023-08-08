# Comparing `tmp/gitlab2zenodo-0.0b4.tar.gz` & `tmp/gitlab2zenodo-0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gitlab2zenodo-0.0b4.tar", last modified: Fri Nov 11 15:22:40 2022, max compression
+gzip compressed data, was "dist/gitlab2zenodo-0.0b5.tar", last modified: Tue Aug  8 11:35:05 2023, max compression
```

## Comparing `gitlab2zenodo-0.0b4.tar` & `gitlab2zenodo-0.0b5.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 sacha     (1000) sacha     (1000)        0 2022-11-11 15:22:40.289654 gitlab2zenodo-0.0b4/
--rw-r--r--   0 sacha     (1000) sacha     (1000)    11345 2020-09-23 08:03:56.000000 gitlab2zenodo-0.0b4/LICENSE
--rw-rw-r--   0 sacha     (1000) sacha     (1000)     8568 2022-11-11 15:22:40.289654 gitlab2zenodo-0.0b4/PKG-INFO
--rw-rw-r--   0 sacha     (1000) sacha     (1000)     7764 2022-11-11 13:17:11.000000 gitlab2zenodo-0.0b4/README.md
-drwxrwxr-x   0 sacha     (1000) sacha     (1000)        0 2022-11-11 15:22:40.285654 gitlab2zenodo-0.0b4/gitlab2zenodo/
--rw-r--r--   0 sacha     (1000) sacha     (1000)        0 2020-09-20 09:43:49.000000 gitlab2zenodo-0.0b4/gitlab2zenodo/__init__.py
--rw-rw-r--   0 sacha     (1000) sacha     (1000)     6353 2022-11-11 15:21:11.000000 gitlab2zenodo-0.0b4/gitlab2zenodo/deposit.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1606 2020-10-13 08:29:11.000000 gitlab2zenodo-0.0b4/gitlab2zenodo/main.py
-drwxrwxr-x   0 sacha     (1000) sacha     (1000)        0 2022-11-11 15:22:40.289654 gitlab2zenodo-0.0b4/gitlab2zenodo.egg-info/
--rw-r--r--   0 sacha     (1000) sacha     (1000)     8568 2022-11-11 15:22:40.000000 gitlab2zenodo-0.0b4/gitlab2zenodo.egg-info/PKG-INFO
--rw-r--r--   0 sacha     (1000) sacha     (1000)      369 2022-11-11 15:22:40.000000 gitlab2zenodo-0.0b4/gitlab2zenodo.egg-info/SOURCES.txt
--rw-r--r--   0 sacha     (1000) sacha     (1000)        1 2022-11-11 15:22:40.000000 gitlab2zenodo-0.0b4/gitlab2zenodo.egg-info/dependency_links.txt
--rw-r--r--   0 sacha     (1000) sacha     (1000)      112 2022-11-11 15:22:40.000000 gitlab2zenodo-0.0b4/gitlab2zenodo.egg-info/entry_points.txt
--rw-r--r--   0 sacha     (1000) sacha     (1000)       19 2022-11-11 15:22:40.000000 gitlab2zenodo-0.0b4/gitlab2zenodo.egg-info/requires.txt
--rw-r--r--   0 sacha     (1000) sacha     (1000)       20 2022-11-11 15:22:40.000000 gitlab2zenodo-0.0b4/gitlab2zenodo.egg-info/top_level.txt
--rw-rw-r--   0 sacha     (1000) sacha     (1000)       38 2022-11-11 15:22:40.289654 gitlab2zenodo-0.0b4/setup.cfg
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1319 2022-11-11 15:21:56.000000 gitlab2zenodo-0.0b4/setup.py
-drwxrwxr-x   0 sacha     (1000) sacha     (1000)        0 2022-11-11 15:22:40.289654 gitlab2zenodo-0.0b4/tests/
--rw-r--r--   0 sacha     (1000) sacha     (1000)        0 2020-09-20 09:43:49.000000 gitlab2zenodo-0.0b4/tests/__init__.py
--rw-rw-r--   0 sacha     (1000) sacha     (1000)    12393 2022-11-11 14:57:20.000000 gitlab2zenodo-0.0b4/tests/test_gitlab2zenodo.py
+drwxrwxr-x   0 sacha     (1000) sacha     (1000)        0 2023-08-08 11:35:05.145534 gitlab2zenodo-0.0b5/
+-rw-r--r--   0 sacha     (1000) sacha     (1000)    11345 2020-09-23 08:03:56.000000 gitlab2zenodo-0.0b5/LICENSE
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)     9848 2023-08-08 11:35:05.145534 gitlab2zenodo-0.0b5/PKG-INFO
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)     7999 2023-06-12 13:12:14.000000 gitlab2zenodo-0.0b5/README.md
+drwxrwxr-x   0 sacha     (1000) sacha     (1000)        0 2023-08-08 11:35:05.145534 gitlab2zenodo-0.0b5/gitlab2zenodo/
+-rw-r--r--   0 sacha     (1000) sacha     (1000)        0 2020-09-20 09:43:49.000000 gitlab2zenodo-0.0b5/gitlab2zenodo/__init__.py
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)     6439 2023-08-08 09:31:41.000000 gitlab2zenodo-0.0b5/gitlab2zenodo/deposit.py
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)     3879 2023-06-16 21:50:35.000000 gitlab2zenodo-0.0b5/gitlab2zenodo/main.py
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)     3711 2023-06-16 10:16:09.000000 gitlab2zenodo-0.0b5/gitlab2zenodo/settings.py
+drwxrwxr-x   0 sacha     (1000) sacha     (1000)        0 2023-08-08 11:35:05.145534 gitlab2zenodo-0.0b5/gitlab2zenodo.egg-info/
+-rw-r--r--   0 sacha     (1000) sacha     (1000)     9848 2023-08-08 11:35:05.000000 gitlab2zenodo-0.0b5/gitlab2zenodo.egg-info/PKG-INFO
+-rw-r--r--   0 sacha     (1000) sacha     (1000)      437 2023-08-08 11:35:05.000000 gitlab2zenodo-0.0b5/gitlab2zenodo.egg-info/SOURCES.txt
+-rw-r--r--   0 sacha     (1000) sacha     (1000)        1 2023-08-08 11:35:05.000000 gitlab2zenodo-0.0b5/gitlab2zenodo.egg-info/dependency_links.txt
+-rw-r--r--   0 sacha     (1000) sacha     (1000)      112 2023-08-08 11:35:05.000000 gitlab2zenodo-0.0b5/gitlab2zenodo.egg-info/entry_points.txt
+-rw-r--r--   0 sacha     (1000) sacha     (1000)       19 2023-08-08 11:35:05.000000 gitlab2zenodo-0.0b5/gitlab2zenodo.egg-info/requires.txt
+-rw-r--r--   0 sacha     (1000) sacha     (1000)       20 2023-08-08 11:35:05.000000 gitlab2zenodo-0.0b5/gitlab2zenodo.egg-info/top_level.txt
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)       38 2023-08-08 11:35:05.145534 gitlab2zenodo-0.0b5/setup.cfg
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)     1439 2023-08-08 10:49:07.000000 gitlab2zenodo-0.0b5/setup.py
+drwxrwxr-x   0 sacha     (1000) sacha     (1000)        0 2023-08-08 11:35:05.145534 gitlab2zenodo-0.0b5/tests/
+-rw-r--r--   0 sacha     (1000) sacha     (1000)        0 2020-09-20 09:43:49.000000 gitlab2zenodo-0.0b5/tests/__init__.py
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)    14861 2023-08-08 11:29:38.000000 gitlab2zenodo-0.0b5/tests/test_gitlab2zenodo.py
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)     6042 2023-08-08 09:31:41.000000 gitlab2zenodo-0.0b5/tests/test_main.py
+-rw-rw-r--   0 sacha     (1000) sacha     (1000)     4541 2023-06-12 13:12:14.000000 gitlab2zenodo-0.0b5/tests/test_settings.py
```

### Comparing `gitlab2zenodo-0.0b4/LICENSE` & `gitlab2zenodo-0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab2zenodo-0.0b4/PKG-INFO` & `gitlab2zenodo-0.0b5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: gitlab2zenodo
-Version: 0.0b4
-Summary: Sends gitlab snapshots to zenodo Automatically.
-Home-page: https://gitlab.com/sbeniamine/gitlab2zenodo
-Author: Sacha Beniamine
-License: Apache License Version 2.0
-Keywords: zenodo gitlab
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![coverage report](https://gitlab.com/sbeniamine/gitlab2zenodo/badges/master/coverage.svg)](https://gitlab.com/sbeniamine/gitlab2zenodo/-/commits/master)
 [![pipeline status](https://gitlab.com/sbeniamine/gitlab2zenodo/badges/master/pipeline.svg)](https://gitlab.com/sbeniamine/gitlab2zenodo/-/commits/master)
 
 
 # Make your code and data citable with Zenodo and Gitlab!
 
 **This script is still in beta ! Please signal any issues you encounter.**
@@ -61,15 +39,15 @@
     - Expand the Variable tab.
     - Click "Add Variable"
     - Enter `zenodo_token` as the variable name and the token as a value.
     - Because this token would allow anyone to push versions and deposits to zenodo, you should check both "Protect" and "Mask".
     - This means that you need to define **protected tags**, that is, tags which only some users can create, and for which the pipelines have access to the token. 
         + This happens in Settings > Repository > Protected Tags. 
         + I use "v*" (and call version tags "v1.0.0", etc). 
-        + Enter the wilcard you want, then click "create wildcard", 
+        + Enter the wildcard you want, then click "create wildcard", 
         + select the users which can create these tags, then click "Protect".
 
 4. If you already have a zenodo record for this repository, add a second variable, with the name `zenodo_record` and the digits of the initial zenodo record as a number. 
 This number is the last part of your DOI (10.5072/zenodo.**123456**). This is used by gitlab2zenodo in order to know which record to update with new versions.
     - If you do not have a zenodo record yet, the first time gitlab2zenodo is triggered, it will create one. You should then add the identifier of this new record as a gitlab variable.
 
 5. Create a `.zenodo.json` file, and fill-in any metadata you want to pass to zenodo. 
@@ -78,16 +56,15 @@
  - unless you define these values in `.zenodo.json`, gitlab2zenodo will add two relations pointing to the repository: 
     - compiled by: the url of your overall repository
     - identical to: the url of the specific tag which is being uploaded
  - If you already have a zenodo deposit with full metadata for the repository, you can use gitlab2zenodo to retrieve the existing metadata:
  
 ~~~
     pip install gitlab2zenodo
-    export zenodo_token="[insert you token here]"
-    g2z-get-meta [your repository ID] > .zenodo.json
+    g2z-get-meta -i [your repository ID] -t [your zenodo token] > .zenodo.json
 ~~~
 
  - Here is a basic example of `.zenodo.json` file, taken from the zenodo api documentation:
  
 ~~~
 {
          'title': 'My first upload',
@@ -105,18 +82,19 @@
 
 send-snapshot:
   rules:
     - if: $CI_COMMIT_TAG =~ /^v?[0-9]+\.[0-9]+/
   script:
     - pip install gitlab2zenodo
     - git archive --format zip --output ${CI_COMMIT_TAG#v}.zip ${CI_COMMIT_TAG}
-    - g2z-send -s -m .zenodo.json ${CI_COMMIT_TAG#v}.zip
+    - g2z-send -i $zenodo_record -t $zenodo_token -s -m .zenodo.json ${CI_COMMIT_TAG#v}.zip
 ~~~
 
 7. Add these lines to your `.gitattributes`, or create one if there is none. This is so that we do not upload these files to zenodo:
+
 ~~~
 .zenodo.json       export-ignore
 .gitlab-ci.yml     export-ignore
 ~~~
 
 # Usage
 
@@ -125,32 +103,30 @@
 The metadata of the new deposit or version will be updated using the current version of your `.zenodo.json` file.
 
 Unless you used the `-p` tag, you should now go to zenodo, review the submitted snapshot, then publish it when it is ready.
 
 If there was no prior zenodo deposit for this repository, one will be created at the first upload. 
 **Go back to add it as a variable, so that the next tags create new versions on zenodo.**
 
-Note that gitlab2zenodo will not create a new version if there is already an unpublished zenodo record. YThe only two possibilities are creating a first deposit with zenodo, or adding a new version for an existing deposit (with no unpublished versions).
-
+Note that gitlab2zenodo will not create a new version if there is already an unpublished zenodo record. 
+The only two possibilities are creating a first deposit with zenodo, or adding a new version for an existing deposit (with no unpublished versions).
 
 ## A walk-through the pipeline file
 
 
 Here is a line-by-line walk through the suggested pipeline file:
-- `image: python:3.6` requires a docker image intended for python3.6
-- `rules`: specify when to run the pipeline
+- `image: python:3.6` requires a docker image intended for python3.6.
+- `rules`: specify when to run the pipeline.
 - `- if: $CI_COMMIT_TAG =~ /^v?[0-9]+\.[0-9]+/`: run only when CI_COMMIT_TAG is given (new tag triggered pipeline), and the tag looks like a version number. The regex assumes that a version number starts with a sequence of a number and a dot, any times, maybe preceded by "v".
 You can change it to your liking if your version numbers follow a different syntax. 
-Note that gitlab2zenodo sets the new version number in the metadata following a similar regex
+Note that gitlab2zenodo sets the new version number in the metadata following a similar regex.
 - `send-snapshot:` is the name of the job we define. The name can be changed, it is not important.
 - `script:` defines the list of command which are executed as this job.
-- `pip install gitlab2zenodo` installs this package
+- `pip install gitlab2zenodo` installs this package,
 - `git archive --format zip --output ${CI_COMMIT_TAG#v}.zip ${CI_COMMIT_TAG}` creates the archive to be uploaded. The name is that of the tag, minus any initial "v".
-- `g2z-send -s -m .zenodo.json ${CI_COMMIT_TAG#v}.zip` sends the archive to zenodo.
-    - `-s` ensures that you send only to zenodo's sandbox
+- `- g2z-send -i $zenodo_record -t $zenodo_token -s -m .zenodo.json ${CI_COMMIT_TAG#v}.zip` sends the archive to zenodo.
+    - `-i` the zenodo record to send the snapshot to. The record ID can also be given directly.
+    - `-t` the zenodo token - this should always be passed as an environment variable.
+    - `-s` ensures that you send only to zenodo's sandbox.
     - `-m .zenodo.json` provides the input file for the metadata. It could be any other json file.
     - by default, this will send a snapshot and edit metadata, but NOT publish. You can ensure publication by adding `-p`, 
     but beware: this can not be undone and files can not be edited after publication.
-
-
-
-
```

### Comparing `gitlab2zenodo-0.0b4/gitlab2zenodo/deposit.py` & `gitlab2zenodo-0.0b5/gitlab2zenodo/deposit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,41 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-import requests
-import os
-import re
+
 import json
-from pathlib import Path
 import logging
+from pathlib import Path
+
+import requests
+
+from gitlab2zenodo.settings import Settings
+
 
 class ZenodoDeposit(object):
     def __init__(self, token=None, sandbox=True):
         self.params = {}
         if token is not None:
             self.params['access_token'] = token
         sandbox_api = "https://sandbox.zenodo.org/api/deposit/depositions"
         normal_api = "https://zenodo.org/api/deposit/depositions"
         self.zenodo_url = sandbox_api if sandbox else normal_api
         self.deposit = None
         self.deposition_id = None
-        self.latest = None
         self.headers = {"Content-Type": "application/json"}
+        self.links = {}
+
+    def _latest_id(self):
+        if not self.links:
+            return self.deposit["id"]
+        if "latest_draft" in self.links:
+            # grab the last unpublished version
+            link = self.links["latest_draft"]
+        else:
+            link = self.links["latest"]
+        return Path(link).name
 
     def _request(self, method, path, full_path=False, **kwargs):
         if not full_path:
             path = self.zenodo_url + path
 
         r = requests.request(method, path,
                              params=self.params,
@@ -32,145 +45,148 @@
         try:
             infos = r.json()
         except:
             try:
                 r.raise_for_status()
             except Exception as e:
                 errors = infos.get("errors", [])
-                extra_message = "".join([err["field"]+": "+err["message"] for err in errors])
+                extra_message = "".join([err["field"] + ": " + err["message"] for err in errors])
                 extra_message += "\n\tThis error occured while sending metadata:\n\t" + str(kwargs)
                 raise requests.RequestException(extra_message) from e
+        if not r.ok:
+            raise requests.RequestException(", ".join([f"{k}: {v}" for k, v in r.json().items()]))
 
         return infos
 
     def get_deposit(self, id):
         logging.info("get deposit")
         r = self._request("GET", "/" + id)
         self.deposition_id = str(r['id'])
         self.links = r["links"]
-        if "latest_draft" in r["links"]:  # grab the last unpublished version
-            self.latest = r["links"]["latest_draft"]
-        else:
-            self.latest = r["links"]["latest"]
         self.deposit = r
         return r
 
     def new_deposit(self):
         logging.info("new deposit")
-        r = self._request("POST", "", json={}) #, headers=self.headers)
+        r = self._request("POST", "", json={})  # , headers=self.headers)
         self.deposit = r
         self.deposition_id = str(r['id'])
         self.links = r["links"]
-        self.latest = str(r['id'])
         return r
 
     def upload(self, path):
         logging.info("upload file")
         with path.open("rb") as fp:
-            r = self._request("PUT", self.links["bucket"] + "/" + path.name, full_path=True, data=fp)
+            r = self._request(
+                "PUT", self.links["bucket"] + "/" + path.name, full_path=True, data=fp)
         return r
 
     def upload_metadata(self, metadata):
         logging.info("upload metadata")
-        return self._request("PUT", "/" + self.latest,
-                             data=json.dumps(metadata), headers=self.headers)
+        r = self._request("PUT", "/" + self._latest_id(),
+                          data=json.dumps(metadata), headers=self.headers)
+        if "links" in r:
+            self.links = r["links"]
+        return r
 
     def remove_existing_files(self):
         logging.info("clean")
-        r = self._request("GET",
-                          "/" + self.latest)  # grab the representation for the very last deposit
+        # grab the representation for the very last deposit
+        r = self._request("GET", "/" + self._latest_id())
         for file in r.get("files", []):
             file_id = file["id"]
-            file_url = "/{}/files/{}"
-            r = self._request("DELETE", file_url.format(self.latest, file_id))
+            file_url = f"/{self._latest_id()}/files/{file_id}"
+            r = self._request("DELETE", file_url)
         return r
 
     def new_version(self):
         logging.info("new version")
-        if self.deposit['submitted'] == False or "latest_draft" in self.deposit[
-            "links"]:
+        if self.deposit['submitted'] == False or "latest_draft" in self.links:
             raise ValueError("The deposit has an unpublished version, "
                              "I can not add a new one. "
                              "Please remove or publish the existing version, "
                              "then run again.")
-        req_url = "/{}/actions/newversion"
-        r = self._request("POST", req_url.format(self.deposition_id))
+        req_url = f"/{self.deposition_id}/actions/newversion"
+        r = self._request("POST", req_url)
         if "links" in r:
-            if "latest_draft" in r["links"]:
-                self.latest = Path(r["links"]["latest_draft"]).name
+            self.links = r["links"]
             self.deposit = r
         return r
 
     def publish_latest_draft(self):
-        logging.info("publish {}".format(self.latest))
-        req_url = "/{}/actions/publish"
-        return self._request("POST", req_url.format(self.latest))
-
-
-def get_metadata(args):
-    try:
-        ACCESS_TOKEN = os.environ['zenodo_token']
-    except KeyError:
-        raise EnvironmentError("You need to set the"
-                               "zenodo_token environment variable")
-    deposit = ZenodoDeposit(token=ACCESS_TOKEN, sandbox=args.sandbox)
-    r = deposit.get_deposit(args.id)
-
-def send(args):
-    try:
-        ACCESS_TOKEN = os.environ['zenodo_token']
-    except KeyError:
-        raise EnvironmentError("You need to set your API token in gitlab's "
-                               "zenodo_token environment variable")
-
-    with args.metadata.open("r", encoding="utf-8") as f:
-        metadata = prepare_metadata(json.load(f))
-
-    deposit = ZenodoDeposit(token=ACCESS_TOKEN, sandbox=args.sandbox)
-
-    if "zenodo_record" in os.environ:
-        deposit.get_deposit(os.environ["zenodo_record"])
+        id = self._latest_id()
+        logging.info(f"publish {id}")
+        req_url = f"/{id}/actions/publish"
+        return self._request("POST", req_url)
+
+
+def get_metadata(settings: Settings):
+    sandbox = settings.get("sandbox")
+    token = settings.get("zenodo_token")
+    record = settings.get("zenodo_record")
+
+    if token is None:
+        raise NameError(
+            "You need to set the zenodo_token environment variable, "
+            "or pass the token as argument")
+    if record is None:
+        raise NameError(
+            "You need to set the zenodo_record environment variable, "
+            "or pass the record ID as argument")
+
+    deposit = ZenodoDeposit(token=token, sandbox=sandbox)
+    return deposit.get_deposit(record)
+
+
+def send(settings: Settings):
+    sandbox = settings.get("sandbox")
+    token = settings.get("zenodo_token")
+    record = settings.get("zenodo_record")
+    metadata_path = settings.get("metadata")
+    archive_path = settings.get("archive")
+    publish = settings.get("publish")
+
+    if token is None:
+        raise NameError(
+            "You need to set the zenodo_token environment variable, "
+            "or pass the token as argument")
+
+    with metadata_path.open("r", encoding="utf-8") as f:
+        metadata = prepare_metadata(json.load(f), settings)
+
+    deposit = ZenodoDeposit(token=token, sandbox=sandbox)
+
+    # if "zenodo_record" in os.environ:
+    if record is not None:
+        deposit.get_deposit(record)
         deposit.new_version()
         deposit.remove_existing_files()
     else:
         deposit.new_deposit()
-        logging.info("Please add the identifier {} as a variable"
-              " zenodo_record:".format(deposit.deposition_id))
+        logging.info(f"Please add the identifier {deposit.deposition_id}"
+                     f" as a variable zenodo_record")
 
     deposit.upload_metadata({'metadata': metadata})
-    deposit.upload(args.archive)
+    deposit.upload(archive_path)
 
-    if args.publish:
+    if publish:
         deposit.publish_latest_draft()
 
 
-def prepare_metadata(metadata):
-    version_regex = "^v?([0-9]+(\.[0-9]+)+.*)$"
-    if 'CI_COMMIT_TAG' in os.environ:
-        match = re.match(version_regex, os.environ['CI_COMMIT_TAG'])
-        if match is not None:
-            metadata["version"] = match.group(1)
-        tag = os.environ['CI_COMMIT_TAG']
-    else:
-        tag = os.environ['CI_COMMIT_SHA']
+def prepare_metadata(metadata, settings):
+    version = settings.get("version")
+    if version is not None:
+        metadata["version"] = version
+
+    ident_set = {item["relation"]: item for item in settings.get(
+        "related_identifiers", [])}
 
-    url = os.environ['CI_PROJECT_URL']
-    tag_url = url + '/-/tree/' + tag
-    tag_relation = {'relation': 'isIdenticalTo', 'identifier': tag_url}
-    repo_relation = {'relation': 'isCompiledBy', 'identifier': url}
     if "related_identifiers" in metadata:
-        identifiers = metadata["related_identifiers"]
-        has_compiledby = False
-        has_identicalto = False
-        for link in identifiers:
-            if link["relation"] == 'isCompiledBy':
-                has_compiledby = True
-            elif link["relation"] == "isIdenticalTo":
-                has_identicalto = True
-
-        if not has_compiledby:
-            identifiers.append(repo_relation)
-        if not has_identicalto:
-            identifiers.append(tag_relation)
+        rel_meta = [item["relation"]
+                    for item in metadata["related_identifiers"]]
+
+        for k, v in ident_set.items():
+            if k not in rel_meta:
+                metadata["related_identifiers"].append(v)
     else:
-        metadata["related_identifiers"] = [tag_relation, repo_relation]
+        metadata["related_identifiers"] = settings.get("related_identifiers")
     return metadata
```

### Comparing `gitlab2zenodo-0.0b4/gitlab2zenodo.egg-info/PKG-INFO` & `gitlab2zenodo-0.0b5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,156 +1,153 @@
 Metadata-Version: 2.1
 Name: gitlab2zenodo
-Version: 0.0b4
+Version: 0.0b5
 Summary: Sends gitlab snapshots to zenodo Automatically.
 Home-page: https://gitlab.com/sbeniamine/gitlab2zenodo
 Author: Sacha Beniamine
 License: Apache License Version 2.0
+Description: [![coverage report](https://gitlab.com/sbeniamine/gitlab2zenodo/badges/master/coverage.svg)](https://gitlab.com/sbeniamine/gitlab2zenodo/-/commits/master)
+        [![pipeline status](https://gitlab.com/sbeniamine/gitlab2zenodo/badges/master/pipeline.svg)](https://gitlab.com/sbeniamine/gitlab2zenodo/-/commits/master)
+        
+        
+        # Make your code and data citable with Zenodo and Gitlab!
+        
+        **This script is still in beta ! Please signal any issues you encounter.**
+        
+        Sends snapshots of your gitlab repository to zenodo automatically, for each new version tag.
+        Zenodo provides a DOI for your code or data, which makes it citable.
+        By publishing automatically when creating new versions, you can make sure the zenodo record stays up to date.
+        
+        - Sending snapshots is triggered by the creation of tags with version names (such as "v1.0.0" or "0.2")
+        - You provide the metadata as a json file
+        - If not given any deposit identifier, the program adds a new deposit. 
+        If given a deposit identifier, it creates a new version. See below on how to provide a deposit identifier.
+        - By default, the script sends an archive and metadata, but does not go through with publication, 
+        in order to let you review the changes. You then need to go to zenodo and publish manually.
+         A parameter is available to publish automatically, but use at your own risks.
+        
+        This uses gitlab pipelines, but should be accessible even if you have never used them.
+        
+        # Installation and setup
+        
+        NOTE: At first, I recommend you do this setup using [zenodo's sandbox](https://sandbox.zenodo.org). 
+        You will need to create an account there, even if you already have a normal zenodo account. 
+        You should only generate a real zenodo token, and setup changes to be pushed to zenodo, once you are certain everything is setup correctly.
+        
+        1. Connect to your Zenodo account (or create one if you do not have one yet)
+        
+        2. [Create an API token](https://zenodo.org/account/settings/applications/tokens/new/) on zenodo, 
+        checking deposit write and deposit publish as rights. Copy the string right away, it is shown only once. 
+        If you failed to do this, simply remove the token and create a new one.
+        
+        3. [Create a custom variable in the Gitlab UI](https://docs.gitlab.com/ee/ci/variables/#create-a-custom-variable-in-the-ui) 
+        with the exact name  and the token as a value. 
+        ![Adding a custom variable](token-variable-screenshot.png)
+            - To do this, go to your repository, then in the left bar in Settings > CI/CD. 
+            - Expand the Variable tab.
+            - Click "Add Variable"
+            - Enter `zenodo_token` as the variable name and the token as a value.
+            - Because this token would allow anyone to push versions and deposits to zenodo, you should check both "Protect" and "Mask".
+            - This means that you need to define **protected tags**, that is, tags which only some users can create, and for which the pipelines have access to the token. 
+                + This happens in Settings > Repository > Protected Tags. 
+                + I use "v*" (and call version tags "v1.0.0", etc). 
+                + Enter the wildcard you want, then click "create wildcard", 
+                + select the users which can create these tags, then click "Protect".
+        
+        4. If you already have a zenodo record for this repository, add a second variable, with the name `zenodo_record` and the digits of the initial zenodo record as a number. 
+        This number is the last part of your DOI (10.5072/zenodo.**123456**). This is used by gitlab2zenodo in order to know which record to update with new versions.
+            - If you do not have a zenodo record yet, the first time gitlab2zenodo is triggered, it will create one. You should then add the identifier of this new record as a gitlab variable.
+        
+        5. Create a `.zenodo.json` file, and fill-in any metadata you want to pass to zenodo. 
+        You can check the [documentation for deposit metadata](https://developers.zenodo.org/#deposit-metadata).
+         - gitlab2zenodo will always update the version when sending to zenodo so that it matches the tag name (removing initial "v")
+         - unless you define these values in `.zenodo.json`, gitlab2zenodo will add two relations pointing to the repository: 
+            - compiled by: the url of your overall repository
+            - identical to: the url of the specific tag which is being uploaded
+         - If you already have a zenodo deposit with full metadata for the repository, you can use gitlab2zenodo to retrieve the existing metadata:
+         
+        ~~~
+            pip install gitlab2zenodo
+            g2z-get-meta -i [your repository ID] -t [your zenodo token] > .zenodo.json
+        ~~~
+        
+         - Here is a basic example of `.zenodo.json` file, taken from the zenodo api documentation:
+         
+        ~~~
+        {
+                 'title': 'My first upload',
+                 'upload_type': 'poster',
+                 'description': 'This is my first upload',
+                 'creators': [{'name': 'Doe, John',
+                               'affiliation': 'Zenodo'}]
+        }
+        ~~~
+        
+        6. Create a `.gitlab-ci.yml` file and write the following code. If you already have a pipeline, simply add a job. Make sure python3.6 is available.
+        
+        ~~~
+        image: python:3.6
+        
+        send-snapshot:
+          rules:
+            - if: $CI_COMMIT_TAG =~ /^v?[0-9]+\.[0-9]+/
+          script:
+            - pip install gitlab2zenodo
+            - git archive --format zip --output ${CI_COMMIT_TAG#v}.zip ${CI_COMMIT_TAG}
+            - g2z-send -i $zenodo_record -t $zenodo_token -s -m .zenodo.json ${CI_COMMIT_TAG#v}.zip
+        ~~~
+        
+        7. Add these lines to your `.gitattributes`, or create one if there is none. This is so that we do not upload these files to zenodo:
+        
+        ~~~
+        .zenodo.json       export-ignore
+        .gitlab-ci.yml     export-ignore
+        ~~~
+        
+        # Usage
+        
+        Any tag with a version name, such as "v1.0.0" should send a snapshot of your repo to zenodo. 
+        
+        The metadata of the new deposit or version will be updated using the current version of your `.zenodo.json` file.
+        
+        Unless you used the `-p` tag, you should now go to zenodo, review the submitted snapshot, then publish it when it is ready.
+        
+        If there was no prior zenodo deposit for this repository, one will be created at the first upload. 
+        **Go back to add it as a variable, so that the next tags create new versions on zenodo.**
+        
+        Note that gitlab2zenodo will not create a new version if there is already an unpublished zenodo record. 
+        The only two possibilities are creating a first deposit with zenodo, or adding a new version for an existing deposit (with no unpublished versions).
+        
+        ## A walk-through the pipeline file
+        
+        
+        Here is a line-by-line walk through the suggested pipeline file:
+        - `image: python:3.6` requires a docker image intended for python3.6.
+        - `rules`: specify when to run the pipeline.
+        - `- if: $CI_COMMIT_TAG =~ /^v?[0-9]+\.[0-9]+/`: run only when CI_COMMIT_TAG is given (new tag triggered pipeline), and the tag looks like a version number. The regex assumes that a version number starts with a sequence of a number and a dot, any times, maybe preceded by "v".
+        You can change it to your liking if your version numbers follow a different syntax. 
+        Note that gitlab2zenodo sets the new version number in the metadata following a similar regex.
+        - `send-snapshot:` is the name of the job we define. The name can be changed, it is not important.
+        - `script:` defines the list of command which are executed as this job.
+        - `pip install gitlab2zenodo` installs this package,
+        - `git archive --format zip --output ${CI_COMMIT_TAG#v}.zip ${CI_COMMIT_TAG}` creates the archive to be uploaded. The name is that of the tag, minus any initial "v".
+        - `- g2z-send -i $zenodo_record -t $zenodo_token -s -m .zenodo.json ${CI_COMMIT_TAG#v}.zip` sends the archive to zenodo.
+            - `-i` the zenodo record to send the snapshot to. The record ID can also be given directly.
+            - `-t` the zenodo token - this should always be passed as an environment variable.
+            - `-s` ensures that you send only to zenodo's sandbox.
+            - `-m .zenodo.json` provides the input file for the metadata. It could be any other json file.
+            - by default, this will send a snapshot and edit metadata, but NOT publish. You can ensure publication by adding `-p`, 
+            but beware: this can not be undone and files can not be edited after publication.
+        
 Keywords: zenodo gitlab
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![coverage report](https://gitlab.com/sbeniamine/gitlab2zenodo/badges/master/coverage.svg)](https://gitlab.com/sbeniamine/gitlab2zenodo/-/commits/master)
-[![pipeline status](https://gitlab.com/sbeniamine/gitlab2zenodo/badges/master/pipeline.svg)](https://gitlab.com/sbeniamine/gitlab2zenodo/-/commits/master)
-
-
-# Make your code and data citable with Zenodo and Gitlab!
-
-**This script is still in beta ! Please signal any issues you encounter.**
-
-Sends snapshots of your gitlab repository to zenodo automatically, for each new version tag.
-Zenodo provides a DOI for your code or data, which makes it citable.
-By publishing automatically when creating new versions, you can make sure the zenodo record stays up to date.
-
-- Sending snapshots is triggered by the creation of tags with version names (such as "v1.0.0" or "0.2")
-- You provide the metadata as a json file
-- If not given any deposit identifier, the program adds a new deposit. 
-If given a deposit identifier, it creates a new version. See below on how to provide a deposit identifier.
-- By default, the script sends an archive and metadata, but does not go through with publication, 
-in order to let you review the changes. You then need to go to zenodo and publish manually.
- A parameter is available to publish automatically, but use at your own risks.
-
-This uses gitlab pipelines, but should be accessible even if you have never used them.
-
-# Installation and setup
-
-NOTE: At first, I recommend you do this setup using [zenodo's sandbox](https://sandbox.zenodo.org). 
-You will need to create an account there, even if you already have a normal zenodo account. 
-You should only generate a real zenodo token, and setup changes to be pushed to zenodo, once you are certain everything is setup correctly.
-
-1. Connect to your Zenodo account (or create one if you do not have one yet)
-
-2. [Create an API token](https://zenodo.org/account/settings/applications/tokens/new/) on zenodo, 
-checking deposit write and deposit publish as rights. Copy the string right away, it is shown only once. 
-If you failed to do this, simply remove the token and create a new one.
-
-3. [Create a custom variable in the Gitlab UI](https://docs.gitlab.com/ee/ci/variables/#create-a-custom-variable-in-the-ui) 
-with the exact name  and the token as a value. 
-![Adding a custom variable](token-variable-screenshot.png)
-    - To do this, go to your repository, then in the left bar in Settings > CI/CD. 
-    - Expand the Variable tab.
-    - Click "Add Variable"
-    - Enter `zenodo_token` as the variable name and the token as a value.
-    - Because this token would allow anyone to push versions and deposits to zenodo, you should check both "Protect" and "Mask".
-    - This means that you need to define **protected tags**, that is, tags which only some users can create, and for which the pipelines have access to the token. 
-        + This happens in Settings > Repository > Protected Tags. 
-        + I use "v*" (and call version tags "v1.0.0", etc). 
-        + Enter the wilcard you want, then click "create wildcard", 
-        + select the users which can create these tags, then click "Protect".
-
-4. If you already have a zenodo record for this repository, add a second variable, with the name `zenodo_record` and the digits of the initial zenodo record as a number. 
-This number is the last part of your DOI (10.5072/zenodo.**123456**). This is used by gitlab2zenodo in order to know which record to update with new versions.
-    - If you do not have a zenodo record yet, the first time gitlab2zenodo is triggered, it will create one. You should then add the identifier of this new record as a gitlab variable.
-
-5. Create a `.zenodo.json` file, and fill-in any metadata you want to pass to zenodo. 
-You can check the [documentation for deposit metadata](https://developers.zenodo.org/#deposit-metadata).
- - gitlab2zenodo will always update the version when sending to zenodo so that it matches the tag name (removing initial "v")
- - unless you define these values in `.zenodo.json`, gitlab2zenodo will add two relations pointing to the repository: 
-    - compiled by: the url of your overall repository
-    - identical to: the url of the specific tag which is being uploaded
- - If you already have a zenodo deposit with full metadata for the repository, you can use gitlab2zenodo to retrieve the existing metadata:
- 
-~~~
-    pip install gitlab2zenodo
-    export zenodo_token="[insert you token here]"
-    g2z-get-meta [your repository ID] > .zenodo.json
-~~~
-
- - Here is a basic example of `.zenodo.json` file, taken from the zenodo api documentation:
- 
-~~~
-{
-         'title': 'My first upload',
-         'upload_type': 'poster',
-         'description': 'This is my first upload',
-         'creators': [{'name': 'Doe, John',
-                       'affiliation': 'Zenodo'}]
-}
-~~~
-
-6. Create a `.gitlab-ci.yml` file and write the following code. If you already have a pipeline, simply add a job. Make sure python3.6 is available.
-
-~~~
-image: python:3.6
-
-send-snapshot:
-  rules:
-    - if: $CI_COMMIT_TAG =~ /^v?[0-9]+\.[0-9]+/
-  script:
-    - pip install gitlab2zenodo
-    - git archive --format zip --output ${CI_COMMIT_TAG#v}.zip ${CI_COMMIT_TAG}
-    - g2z-send -s -m .zenodo.json ${CI_COMMIT_TAG#v}.zip
-~~~
-
-7. Add these lines to your `.gitattributes`, or create one if there is none. This is so that we do not upload these files to zenodo:
-~~~
-.zenodo.json       export-ignore
-.gitlab-ci.yml     export-ignore
-~~~
-
-# Usage
-
-Any tag with a version name, such as "v1.0.0" should send a snapshot of your repo to zenodo. 
-
-The metadata of the new deposit or version will be updated using the current version of your `.zenodo.json` file.
-
-Unless you used the `-p` tag, you should now go to zenodo, review the submitted snapshot, then publish it when it is ready.
-
-If there was no prior zenodo deposit for this repository, one will be created at the first upload. 
-**Go back to add it as a variable, so that the next tags create new versions on zenodo.**
-
-Note that gitlab2zenodo will not create a new version if there is already an unpublished zenodo record. YThe only two possibilities are creating a first deposit with zenodo, or adding a new version for an existing deposit (with no unpublished versions).
-
-
-## A walk-through the pipeline file
-
-
-Here is a line-by-line walk through the suggested pipeline file:
-- `image: python:3.6` requires a docker image intended for python3.6
-- `rules`: specify when to run the pipeline
-- `- if: $CI_COMMIT_TAG =~ /^v?[0-9]+\.[0-9]+/`: run only when CI_COMMIT_TAG is given (new tag triggered pipeline), and the tag looks like a version number. The regex assumes that a version number starts with a sequence of a number and a dot, any times, maybe preceded by "v".
-You can change it to your liking if your version numbers follow a different syntax. 
-Note that gitlab2zenodo sets the new version number in the metadata following a similar regex
-- `send-snapshot:` is the name of the job we define. The name can be changed, it is not important.
-- `script:` defines the list of command which are executed as this job.
-- `pip install gitlab2zenodo` installs this package
-- `git archive --format zip --output ${CI_COMMIT_TAG#v}.zip ${CI_COMMIT_TAG}` creates the archive to be uploaded. The name is that of the tag, minus any initial "v".
-- `g2z-send -s -m .zenodo.json ${CI_COMMIT_TAG#v}.zip` sends the archive to zenodo.
-    - `-s` ensures that you send only to zenodo's sandbox
-    - `-m .zenodo.json` provides the input file for the metadata. It could be any other json file.
-    - by default, this will send a snapshot and edit metadata, but NOT publish. You can ensure publication by adding `-p`, 
-    but beware: this can not be undone and files can not be edited after publication.
-
-
-
-
```

### Comparing `gitlab2zenodo-0.0b4/setup.py` & `gitlab2zenodo-0.0b5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from setuptools import setup, find_packages
+import json
 
+with open('.zenodo.json', "r", encoding="utf-8") as f:
+    data = json.load(f)
+    version = data["version"]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='gitlab2zenodo',
     license='Apache License Version 2.0',
-    version='0.0.b4',
+    version=version,
     packages=find_packages(),
     url='https://gitlab.com/sbeniamine/gitlab2zenodo',
     author='Sacha Beniamine',
     install_requires=['requests', 'responses'],
     entry_points = {
         "console_scripts": [
             "g2z-send = gitlab2zenodo.main:g2z_command",
```

### Comparing `gitlab2zenodo-0.0b4/tests/test_gitlab2zenodo.py` & `gitlab2zenodo-0.0b5/tests/test_gitlab2zenodo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from unittest import TestCase
-from unittest.mock import patch, Mock, mock_open
-from types import SimpleNamespace
-from gitlab2zenodo.deposit import ZenodoDeposit, prepare_metadata, send
-import requests
-import responses
+import json
 import re
 from copy import deepcopy
 from functools import partial
 from pathlib import Path
-import json
+from types import SimpleNamespace
+from unittest import TestCase
+from unittest.mock import Mock, mock_open, patch
+import os
+
+import requests
+import responses
+
+from gitlab2zenodo.deposit import ZenodoDeposit, prepare_metadata, send
+from gitlab2zenodo.settings import Settings
 
 metadata_content = {
     "title": "Some title",
     "upload_type": "dataset",
     "description": "This is a test metadata",
     "version": "0.1.0",
     "creators": [
@@ -24,24 +28,27 @@
         }
     ]
 }
 
 
 class TestGitlab2Zenodo(TestCase):
     bucket_link = 'https://sandbox.zenodo.org/api/files/some-sha'
+    bucket_link2 = 'https://sandbox.zenodo.org/api/files/some-other-sha'
     deposit_120 = {'id': '120', 'links': {'latest': '120', 'bucket': bucket_link},
                    'files': [{'id': '7'}], 'submitted': False}
     deposit_123 = {'id': '123', 'links': {'latest': '123', 'bucket': bucket_link},
                    'files': [{'id': '8'}], 'submitted': True}
     deposit_123_draft = {'id': '123', 'links': {'latest_draft': '124', 'bucket': bucket_link},
                          'files': [{'id': '8'}], 'submitted': True}
     deposit_124 = {'id': '124', 'links': {'latest_draft': '124', 'bucket': bucket_link},
                    'files': [{'id': '1'}, {'id': '2'}], 'submitted': True}
-    deposit_345 = {'id': '345', 'links': {'latest_draft': '124','bucket': bucket_link},
+    deposit_345 = {'id': '345', 'links': {'latest_draft': '124', 'bucket': bucket_link},
                    'files': [{'id': '5'}, {'id': '6'}], 'submitted': True}
+    deposit_4 = {'id': 4, 'links': {'bucket': bucket_link2,
+                                    'latest_draft': '3'}}
 
     @classmethod
     def tearDownClass(cls):
         responses.stop()
         responses.reset()
 
     @classmethod
@@ -74,27 +81,29 @@
 
         # test_new_deposit
         responses.add_callback(responses.POST,
                                re.compile(api_regex + authorized_token),
                                callback=partial(force_json,
                                                 json_resp=cls.deposit_120)
                                )
+        responses.add(responses.POST, re.compile(
+            api_regex + "/120/actions/publish" + authorized_token),
+                      status=200)
 
         # test_send
         responses.add_callback(responses.PUT,
                                re.compile(
                                    api_regex + r"/\d+" + authorized_token),
                                callback=force_json)
 
         # test_send, test_upload (using bucket link)
         responses.add(responses.PUT,
-                               re.compile(
-                                   cls.bucket_link + r".+\.(json|zip)" + authorized_token),
-                       status=200)
-
+                      re.compile(
+                          cls.bucket_link + r".+\.(json|zip)" + authorized_token),
+                      status=200)
 
         # test_remove_existing_files
         responses.add(responses.DELETE,
                       re.compile(
                           api_regex + "/124/files/(1|2)" + authorized_token),
                       status=200)
 
@@ -103,14 +112,18 @@
             api_regex + "/(12[34])/actions/newversion" + authorized_token),
                       json=cls.deposit_123_draft,
                       status=200)
         # test_publish_latest_draft
         responses.add(responses.POST, re.compile(
             api_regex + "/124/actions/publish" + authorized_token),
                       status=200)
+        # test upload_metadata updating links to store new bucket
+        responses.add(responses.PUT,
+                      re.compile(api_regex + "/4" + authorized_token),
+                      json=cls.deposit_4, status=200)
 
     def test_send(self):
 
         mock_path = Mock(spec=Path)
         mock_path.open = mock_open(read_data=json.dumps(metadata_content))
         mock_path.name = ".zenodo.json"
 
@@ -119,137 +132,161 @@
         mock_path2.name = ".zenodo.json"
 
         args = SimpleNamespace(sandbox=True, publish=True,
                                metadata=mock_path,
                                archive=mock_path2)
 
         # When no token, throws exception
-        with patch.dict('os.environ', {}):
-            self.assertRaises(EnvironmentError, send, args)
+        with patch.dict('os.environ', {}, clear=True):
+            # We could update the settings directly, but calling the
+            # instantiation re-created the original functionality of
+            # `prepare_metadata()` where environment variables are read
+            settings = Settings(args)
+            self.assertRaises(NameError, send, settings)
 
         # With a proper environment and token, goes through
         env = {"zenodo_record": "123",
                "CI_COMMIT_TAG": "v1.0.1-beta",
                "CI_PROJECT_URL": "https://gitlab.com/user/project",
                "zenodo_token": "test_token"
                }
         with patch.dict('os.environ', env):
+            settings = Settings(args)
             try:
-                send(args)
-                args.publish = False
-                send(args)
+                settings["publish"] = True
+                send(settings)
+                settings["publish"] = False
+                send(settings)
             except:
                 self.fail("Main function failed")
 
         # With a proper environment and no record, goes through
         del env["zenodo_record"]
         with patch.dict('os.environ', env):
+            settings = Settings(args)
             try:
-                send(args)
-                args.publish = False
-                send(args)
+                settings["publish"] = True
+                send(settings)
+                settings["publish"] = False
+                send(settings)
             except:
                 self.fail("Main function failed")
 
-
     def test_prepare_metadata(self):
         env = {"zenodo_record": "123",
                "CI_COMMIT_SHA": "somesha",
                "CI_COMMIT_TAG": "v1.0.1-beta",
                "CI_PROJECT_URL": "https://gitlab.com/user/project"
                }
         metadata = deepcopy(metadata_content)
 
         with patch.dict('os.environ', env):
             # When there were no relations and we have a tag version,
             # Add relations and replace version number
-
-            result = prepare_metadata(deepcopy(metadata))
+            # We could update the settings directly, but calling the
+            # instantiation re-created the original functionality of
+            # `prepare_metadata()` where environment variables are read
+            settings = Settings()
+            result = prepare_metadata(deepcopy(metadata), settings)
             expected = deepcopy(metadata)
             expected.update({'version': '1.0.1-beta',
                              'related_identifiers':
                                  [{'relation': 'isIdenticalTo',
                                    'identifier': 'https://gitlab.com/user/project/-/tree/v1.0.1-beta'},
                                   {'relation': 'isCompiledBy',
                                    'identifier': 'https://gitlab.com/user/project'}]
                              })
             self.assertDictEqual(result, expected)
 
             # When the relations exist already, do not change them.
             idto = {'relation': 'isIdenticalTo', 'identifier': 'itself'}
             metadata['related_identifiers'] = [idto]
-            result = prepare_metadata(deepcopy(metadata))
+            result = prepare_metadata(deepcopy(metadata), settings)
             self.assertIn(idto, result["related_identifiers"])
 
             compiledby = {'relation': 'isCompiledBy', 'identifier': 'a repo'}
             metadata['related_identifiers'] = [compiledby]
-            result = prepare_metadata(deepcopy(metadata))
+            result = prepare_metadata(deepcopy(metadata), settings)
             self.assertIn(compiledby, result["related_identifiers"])
 
+        # When the tag is a version name, change version
+        env["CI_COMMIT_TAG"] = "v2.0.0"
+        settings["version"] = metadata["version"]
+        with patch.dict('os.environ', env):
+            settings = Settings()
+            result = prepare_metadata(deepcopy(metadata), settings)
+            self.assertEqual(result["version"], env["CI_COMMIT_TAG"][1:])
+
         # When the tag is not a version name, do not change version
         env["CI_COMMIT_TAG"] = "test"
+        settings["version"] = metadata["version"]
         with patch.dict('os.environ', env):
-            result = prepare_metadata(deepcopy(metadata))
-            self.assertEqual(result["version"], "0.1.0")
+            settings = Settings()
+            result = prepare_metadata(deepcopy(metadata), settings)
+            self.assertEqual(result["version"], metadata["version"])
 
         # When the commit is not a tag, do not change version
         del env["CI_COMMIT_TAG"]
         with patch.dict('os.environ', env):
-            result = prepare_metadata(deepcopy(metadata))
-            self.assertEqual(result["version"], "0.1.0")
+            # Must be removed here, the patch doesn't remove previous values
+            if "CI_COMMIT_TAG" in os.environ:
+                del os.environ["CI_COMMIT_TAG"]
+            settings = Settings()
+            result = prepare_metadata(deepcopy(metadata), settings)
+            self.assertEqual(result["version"], metadata["version"])
 
     def test_ZenodoDepositObject(self):
         # When creating the object, the sandbox switch changes the url
         deposit = ZenodoDeposit(token="token", sandbox=True)
         self.assertEqual(deposit.zenodo_url,
                          "https://sandbox.zenodo.org/api/deposit/depositions")
         deposit = ZenodoDeposit(token="token", sandbox=False)
         self.assertEqual(deposit.zenodo_url,
                          "https://zenodo.org/api/deposit/depositions")
 
     def test_get_deposit(self):
-        ## Getting fails with a wrong token
+        # Getting fails with a wrong token
         deposit = ZenodoDeposit(token="token", sandbox=True)
         self.assertRaises(requests.exceptions.ConnectionError,
                           deposit.get_deposit, "123")
 
-        ## Fails with a wrong id
+        # Fails with a wrong id
         deposit = ZenodoDeposit(token="test_token", sandbox=True)
         self.assertRaises(requests.exceptions.ConnectionError,
                           deposit.get_deposit, "333")
 
         try:
-            ## But works when using correct test token and existing id
+            # But works when using correct test token and existing id
             deposit = ZenodoDeposit(token="test_token", sandbox=True)
             deposit.get_deposit("123")
         except requests.exceptions.ConnectionError:
             self.fail("Wrong route")
         self.assertEqual(deposit.deposition_id, "123")
-        self.assertEqual(deposit.latest, "123")
+        self.assertEqual(deposit._latest_id(), "123")
         self.assertEqual(deposit.deposit, self.deposit_123)
 
         try:
-            ## with a deposit which has a draft, does find the draft id
+            # with a deposit which has a draft, does find the draft id
             deposit = ZenodoDeposit(token="test_token", sandbox=True)
             deposit.get_deposit("345")
         except requests.exceptions.ConnectionError:
             self.fail("Wrong route")
         self.assertEqual(deposit.deposition_id, "345")
-        self.assertEqual(deposit.latest, "124")
+        self.assertEqual(deposit._latest_id(), "124")
         self.assertEqual(deposit.deposit, self.deposit_345)
 
     def test_new_deposit(self):
         try:
             # When creating a new deposit, all fields are updated
             deposit = ZenodoDeposit(token="test_token", sandbox=True)
             deposit.new_deposit()
         except requests.exceptions.ConnectionError:
             self.fail("Wrong route")
         self.assertEqual(deposit.deposition_id, "120")
-        self.assertEqual(deposit.latest, "120")
+        self.assertEqual(deposit._latest_id(), "120")
         self.assertEqual(deposit.deposit, self.deposit_120)
 
     def test_upload(self):
         try:
             # Upload uses the right route and sends multipart data
             deposit = ZenodoDeposit(token="test_token", sandbox=True)
             deposit.new_deposit()
@@ -266,14 +303,22 @@
         deposit = ZenodoDeposit(token="test_token", sandbox=True)
         deposit.new_deposit()
         try:
             deposit.upload_metadata({'metadata': {"key": "value"}})
         except:
             self.fail("Metadata call failed")
 
+    def test_upload_metadata_updates_links(self):
+        # when depositing metadata, bucket should be updated by storing 'links'
+        deposit = ZenodoDeposit(token="test_token", sandbox=True)
+        deposit.deposit = {"id": "4"}
+        self.assertNotIn('bucket', deposit.links)
+        deposit.upload_metadata({'metadata': {"key": "value"}})
+        self.assertEqual(deposit.links['bucket'], self.bucket_link2)
+
     def test_remove_existing_files(self):
         # Grabs latest version
         try:
             deposit = ZenodoDeposit(token="test_token", sandbox=True)
             deposit.get_deposit("345")
             # getting 345, but latest version, with the right files to delete, is 124
             deposit.remove_existing_files()
@@ -284,15 +329,15 @@
         # Works when latest is published
         try:
             deposit = ZenodoDeposit(token="test_token", sandbox=True)
             deposit.get_deposit("123")
             deposit.new_version()
         except:
             self.fail("New version call on submitted deposit fails")
-        self.assertEqual(deposit.latest, "124")
+        self.assertEqual(deposit._latest_id(), "124")
         self.assertEqual(deposit.deposit, self.deposit_123_draft)
 
         # Should throw when deposit is not published yet
         deposit.new_deposit()
         self.assertRaises(ValueError, deposit.new_version)
 
         # Should throw when deposit is published but has unpublished version
```

