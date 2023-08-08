# Comparing `tmp/idms-0.2.1.tar.gz` & `tmp/idms-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idms-0.2.1.tar", last modified: Thu Jul 13 09:31:42 2023, max compression
+gzip compressed data, was "idms-0.2.3.tar", last modified: Tue Aug  8 08:37:00 2023, max compression
```

## Comparing `idms-0.2.1.tar` & `idms-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-13 09:31:31.000000 idms-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 09:31:31.000000 idms-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-13 09:31:42.876928 idms-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-13 09:31:31.000000 idms-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 09:31:31.000000 idms-0.2.1/data/data_file
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 09:31:31.000000 idms-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 09:31:42.880928 idms-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-13 09:31:31.000000 idms-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/idms/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 09:31:31.000000 idms-0.2.1/src/idms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/idms/api/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 09:31:31.000000 idms-0.2.1/src/idms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-07-13 09:31:31.000000 idms-0.2.1/src/idms/api/contentserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 09:31:31.000000 idms-0.2.1/src/idms/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/idms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 09:31:42.000000 idms-0.2.1/src/idms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:31:42.876928 idms-0.2.1/src/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 09:31:31.000000 idms-0.2.1/src/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 09:31:31.000000 idms-0.2.1/src/sample/package_data.dat
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 09:31:31.000000 idms-0.2.1/src/sample/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:37:00.465005 idms-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-08 08:36:51.000000 idms-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-08 08:36:51.000000 idms-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-08 08:37:00.465005 idms-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-08 08:36:51.000000 idms-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:37:00.465005 idms-0.2.3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 08:36:51.000000 idms-0.2.3/data/data_file
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-08 08:36:51.000000 idms-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 08:37:00.465005 idms-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-08-08 08:36:51.000000 idms-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:37:00.461005 idms-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:37:00.465005 idms-0.2.3/src/idms/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 08:36:51.000000 idms-0.2.3/src/idms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:37:00.465005 idms-0.2.3/src/idms/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 08:36:51.000000 idms-0.2.3/src/idms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-08-08 08:36:51.000000 idms-0.2.3/src/idms/api/contentserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-08 08:36:51.000000 idms-0.2.3/src/idms/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:37:00.465005 idms-0.2.3/src/idms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-08 08:37:00.000000 idms-0.2.3/src/idms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 08:37:00.000000 idms-0.2.3/src/idms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 08:37:00.000000 idms-0.2.3/src/idms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 08:37:00.000000 idms-0.2.3/src/idms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 08:37:00.000000 idms-0.2.3/src/idms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 08:37:00.000000 idms-0.2.3/src/idms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:37:00.465005 idms-0.2.3/src/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 08:36:51.000000 idms-0.2.3/src/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 08:36:51.000000 idms-0.2.3/src/sample/package_data.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 08:36:51.000000 idms-0.2.3/src/sample/simple.py
```

### Comparing `idms-0.2.1/LICENSE.txt` & `idms-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `idms-0.2.1/PKG-INFO` & `idms-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.2.1
+Version: 0.2.3
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
 Home-page: https://github.com/Provincie-Zuid-Holland/idms
-Author: Daniel Overdevest
-Author-email: d.overdevest@pzh.nl
+Author: Daniel Overdevest, Michael de Winter
+Author-email: d.overdevest@pzh.nl, mr.de.winter@pzh.nl
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
 Keywords: idms,contentserver,restapi,searchapi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `idms-0.2.1/README.md` & `idms-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `idms-0.2.1/setup.py` & `idms-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="idms",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.2.1",  # Required
+    version="0.2.3",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Python class to talk to idms REST and Search API, better known as iDMS.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -64,18 +64,18 @@
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
     url="https://github.com/Provincie-Zuid-Holland/idms",  # Optional
     # This should be your name or the name of the organization which owns the
     # project.
-    author="Daniel Overdevest",  # Optional
+    author="Daniel Overdevest, Michael de Winter",  # Optional
     # This should be a valid email address corresponding to the author listed
     # above.
-    author_email="d.overdevest@pzh.nl",  # Optional
+    author_email="d.overdevest@pzh.nl, mr.de.winter@pzh.nl",  # Optional
     # Classifiers help users find your project by categorizing it.
     #
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
```

### Comparing `idms-0.2.1/src/idms/api/contentserver.py` & `idms-0.2.3/src/idms/api/contentserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     def __init__(
         self,
         baseUrl: str,
         username: str = None,
         password: str = None,
         ticket: str = None,
         verifySSL: bool = True,
+        maxErrorRetry: int = 30
     ):
         # Settings for retry and auto retry if error code 500 is given
         retry = Retry(
             total=5,
             read=5,
             connect=5,
             backoff_factor=0.3,
@@ -78,14 +79,17 @@
             "properties.description_multilingual.nl",
             "regions.OTLocation",
             "systemattributes.Dossiernummer",
         ]
 
         self.debugJson = False
 
+        # Retry faulty urls
+        self.maxErrorRetry = maxErrorRetry
+
         if ticket:
             self.ticket = ticket
         else:
             self.ticket = self.authorize(username, password)
 
     def authorize(self, username: str, password: str) -> str:
         """
@@ -247,63 +251,82 @@
 
         :param str `complexQuery`:  See documentation for search options for a complexQuery: https://docs2.cer-rec.gc.ca/ll-eng/llisapi.dll?func=help.index&keyword=LL.Search%20Broker.Category
         """
         results = []
         headers = {"otcsticket": self.ticket}
         counter = 0
         url = self.baseUrl + "/api/v2/search"
+        max_error_retries = 0
 
         base_data = {"where": complexQuery, "limit": limit, "metadata": metadata}
         if slice:
             base_data["slice"] = slice
 
         # Retrieve all pages of certain search query using a while loop with security of maxCallsPerFolder variable.
-        while url != "" and counter < self.maxCallsPerFolder:
-            counter = counter + 1
-            data = base_data.copy()
-            # Query Content Server API to search for params
-            if "?" in url:
-                url, params = url.split("?")
-
-                # Split the query string on the '&' character
-                query_params = params.split('&')
-
-                # Loop through each key-value pair and add it to the dictionary
-                for param in query_params:
-                    key, value = param.split('=')
-                    data[key] = value
-
-            logging.debug(data)
-            r = self.session.post(url, headers=headers, timeout=60 * 30, data=data)
-            r.raise_for_status()
-            search_results = r.json()
-            if self.debugJson:
-                yyyymmddhhmmss = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
-                with open(f"debug_{yyyymmddhhmmss}.json", "w") as f:
-                    json.dump(search_results, f)
-
-            # Extract only relevant columns from search results
-            for result in search_results.get("results", []):
-                dataRow = result.get("data")
-                row = self.parseNodeColumns(dataRow)
-
-                ancestorsList = dotfield(result, "links.ancestors", [])
-                ancestorsStr = " > ".join([a.get("name") for a in ancestorsList])
-                row["locationPathString"] = ancestorsStr
-                row["complexQuery"] = complexQuery
-                results.append(row)
-
-            # Determine if there is a next page and prepare for next while-loop.
-            # nextUrl contains a GET url to retrieve the next page.
-            nextUrl = dotfield(search_results, "collection.paging.links.next.href")
-            logging.debug(f" > nextUrl: {nextUrl}")
-            if nextUrl:
-                url = self.baseUrl + nextUrl
-            else:
-                url = ""
+        while url != "" and counter < self.maxCallsPerFolder and max_error_retries < self.maxErrorRetry:
+            try:
+                counter = counter + 1
+                data = base_data.copy()
+                # Query Content Server API to search for params
+                if "?" in url:
+                    url, params = url.split("?")
+
+                    # Split the query string on the '&' character
+                    query_params = params.split('&')
+
+                    # Loop through each key-value pair and add it to the dictionary
+                    for param in query_params:
+                        key, value = param.split('=')
+                        data[key] = value
+
+                logging.debug(data)
+
+                # The post might sometimes fail thus stop the whole process, i have added a retry if the post fails to try again, this seems to work
+                r = self.session.post(url, headers=headers, timeout=60 * 30, data=data)             
+                r.raise_for_status()
+                search_results = r.json()
+
+
+                if self.debugJson:
+                    yyyymmddhhmmss = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
+                    with open(f"debug_{yyyymmddhhmmss}.json", "w") as f:
+                        json.dump(search_results, f)
+
+                # Extract only relevant columns from search results
+                for result in search_results.get("results", []):
+                    dataRow = result.get("data")
+                    row = self.parseNodeColumns(dataRow)
+
+                    ancestorsList = dotfield(result, "links.ancestors", [])
+                    ancestorsStr = " > ".join([a.get("name") for a in ancestorsList])
+                    row["locationPathString"] = ancestorsStr
+                    row["complexQuery"] = complexQuery
+                    results.append(row)
+
+                # Determine if there is a next page and prepare for next while-loop.
+                # nextUrl contains a GET url to retrieve the next page.
+                nextUrl = dotfield(search_results, "collection.paging.links.next.href")
+               
+                logging.debug(f" > nextUrl: {nextUrl}")
+
+                if nextUrl:
+                    url = self.baseUrl + nextUrl
+                else:
+                    url = ""
+
+            except Exception as e:              
+                    max_error_retries = max_error_retries+1
+                    print(e)
+                    logging.debug("Error: "+str(e))
+
+        # Inform the user that the max error retries has been met.
+        if max_error_retries >= self.maxErrorRetry:
+              logging.warning(
+                f"Stopped due max error tries: ({max_error_retries}) reached the max error retry ({self.maxErrorRetry}) limit!"
+            )
 
         # Inform user if stopped earlier due maxCallsPerFolder variable
         if counter >= self.maxCallsPerFolder:
             logging.warning(
                 f"Stopped due counter ({counter}) reached the maxCallsPerFolder ({self.maxCallsPerFolder}) limit!"
             )
```

### Comparing `idms-0.2.1/src/idms/functions.py` & `idms-0.2.3/src/idms/functions.py`

 * *Files identical despite different names*

### Comparing `idms-0.2.1/src/idms.egg-info/PKG-INFO` & `idms-0.2.3/src/idms.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.2.1
+Version: 0.2.3
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
 Home-page: https://github.com/Provincie-Zuid-Holland/idms
-Author: Daniel Overdevest
-Author-email: d.overdevest@pzh.nl
+Author: Daniel Overdevest, Michael de Winter
+Author-email: d.overdevest@pzh.nl, mr.de.winter@pzh.nl
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
 Keywords: idms,contentserver,restapi,searchapi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

