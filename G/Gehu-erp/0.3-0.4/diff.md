# Comparing `tmp/Gehu_erp-0.3.tar.gz` & `tmp/Gehu_erp-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Gehu_erp-0.3.tar", last modified: Mon Aug  7 18:50:00 2023, max compression
+gzip compressed data, was "Gehu_erp-0.4.tar", last modified: Tue Aug  8 18:25:34 2023, max compression
```

## Comparing `Gehu_erp-0.3.tar` & `Gehu_erp-0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 18:50:00.501825 Gehu_erp-0.3/
-drwxrwxrwx   0        0        0        0 2023-08-07 18:50:00.498278 Gehu_erp-0.3/Gehu_erp.egg-info/
--rw-rw-rw-   0        0        0     2112 2023-08-07 18:50:00.000000 Gehu_erp-0.3/Gehu_erp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-08-07 18:50:00.000000 Gehu_erp-0.3/Gehu_erp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 18:50:00.000000 Gehu_erp-0.3/Gehu_erp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-08-07 18:50:00.000000 Gehu_erp-0.3/Gehu_erp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-07 18:50:00.000000 Gehu_erp-0.3/Gehu_erp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2112 2023-08-07 18:50:00.501825 Gehu_erp-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1746 2023-08-07 18:48:23.000000 Gehu_erp-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 18:50:00.501825 Gehu_erp-0.3/erp/
--rw-rw-rw-   0        0        0       71 2023-08-07 17:14:37.000000 Gehu_erp-0.3/erp/__init__.py
--rw-rw-rw-   0        0        0     3309 2023-08-07 18:47:25.000000 Gehu_erp-0.3/erp/client.py
-drwxrwxrwx   0        0        0        0 2023-08-07 18:50:00.501825 Gehu_erp-0.3/erp/util/
--rw-rw-rw-   0        0        0       22 2023-08-07 17:14:02.000000 Gehu_erp-0.3/erp/util/__init__.py
--rw-rw-rw-   0        0        0     1903 2023-08-07 16:45:38.000000 Gehu_erp-0.3/erp/util/headers.py
--rw-rw-rw-   0        0        0       42 2023-08-07 18:50:00.501825 Gehu_erp-0.3/setup.cfg
--rw-rw-rw-   0        0        0      721 2023-08-07 18:49:35.000000 Gehu_erp-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:25:34.727017 Gehu_erp-0.4/
+drwxrwxrwx   0        0        0        0 2023-08-08 18:25:34.680143 Gehu_erp-0.4/Gehu_erp.egg-info/
+-rw-rw-rw-   0        0        0     2256 2023-08-08 18:25:34.000000 Gehu_erp-0.4/Gehu_erp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-08-08 18:25:34.000000 Gehu_erp-0.4/Gehu_erp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 18:25:34.000000 Gehu_erp-0.4/Gehu_erp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-08-08 18:25:34.000000 Gehu_erp-0.4/Gehu_erp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-08 18:25:34.000000 Gehu_erp-0.4/Gehu_erp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2256 2023-08-08 18:25:34.727017 Gehu_erp-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1879 2023-08-08 18:24:55.000000 Gehu_erp-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 18:25:34.695771 Gehu_erp-0.4/erp/
+-rw-rw-rw-   0        0        0       95 2023-08-08 14:58:55.000000 Gehu_erp-0.4/erp/__init__.py
+-rw-rw-rw-   0        0        0     5865 2023-08-08 17:42:37.000000 Gehu_erp-0.4/erp/client.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:25:34.727017 Gehu_erp-0.4/erp/util/
+-rw-rw-rw-   0        0        0       45 2023-08-08 14:57:57.000000 Gehu_erp-0.4/erp/util/__init__.py
+-rw-rw-rw-   0        0        0     1339 2023-08-08 15:08:56.000000 Gehu_erp-0.4/erp/util/config.py
+-rw-rw-rw-   0        0        0     1966 2023-08-08 16:51:49.000000 Gehu_erp-0.4/erp/util/headers.py
+-rw-rw-rw-   0        0        0       42 2023-08-08 18:25:34.727017 Gehu_erp-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-08-08 18:24:02.000000 Gehu_erp-0.4/setup.py
```

### Comparing `Gehu_erp-0.3/Gehu_erp.egg-info/PKG-INFO` & `Gehu_erp-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: Gehu-erp
-Version: 0.3
+Name: Gehu_erp
+Version: 0.4
 Summary: A Python library for interacting with GEHU Student API
-Home-page: https://github.com/aminobot22
+Home-page: https://github.com/aminobot22/gehu_erp
 Author: yato
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Gehu_erp - A Python Library for Interacting with GEHU Student API
@@ -47,14 +47,18 @@
 ## Setup and Installation
 
 To use Gehu_erp, you need to install it via pip. First, ensure you have Python installed, then open a terminal and run the following command:
 
 ```
 pip install Gehu_erp
 ```
+## Docs
+
+For more information and examples, please visit the [documentation](https://gehu-erp.readthedocs.io/en/latest/index.html).
+
 
 ## Dependencies
 
 Gehu_erp depends on the following Python libraries:
 - requests
 - Pillow
 - beautifulsoup4
@@ -68,9 +72,8 @@
 ## Contributing
 
 If you would like to contribute to Gehu_erp, feel free to submit a pull request or open an issue on the GitHub repository.
 
 ## Acknowledgments
 
 - Thanks to the developers of `requests`, `Pillow`, and `beautifulsoup4` for their excellent libraries.
-- Special thanks to the developers and maintainers of the GEHU Student API for providing the API that this library interacts with.
-```
+- Special thanks to the developers and maintainers of the GEHU Student API for providing the API that this library interacts with.```
```

### Comparing `Gehu_erp-0.3/PKG-INFO` & `Gehu_erp-0.4/Gehu_erp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: Gehu_erp
-Version: 0.3
+Name: Gehu-erp
+Version: 0.4
 Summary: A Python library for interacting with GEHU Student API
-Home-page: https://github.com/aminobot22
+Home-page: https://github.com/aminobot22/gehu_erp
 Author: yato
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Gehu_erp - A Python Library for Interacting with GEHU Student API
@@ -47,14 +47,18 @@
 ## Setup and Installation
 
 To use Gehu_erp, you need to install it via pip. First, ensure you have Python installed, then open a terminal and run the following command:
 
 ```
 pip install Gehu_erp
 ```
+## Docs
+
+For more information and examples, please visit the [documentation](https://gehu-erp.readthedocs.io/en/latest/index.html).
+
 
 ## Dependencies
 
 Gehu_erp depends on the following Python libraries:
 - requests
 - Pillow
 - beautifulsoup4
@@ -68,9 +72,8 @@
 ## Contributing
 
 If you would like to contribute to Gehu_erp, feel free to submit a pull request or open an issue on the GitHub repository.
 
 ## Acknowledgments
 
 - Thanks to the developers of `requests`, `Pillow`, and `beautifulsoup4` for their excellent libraries.
-- Special thanks to the developers and maintainers of the GEHU Student API for providing the API that this library interacts with.
-```
+- Special thanks to the developers and maintainers of the GEHU Student API for providing the API that this library interacts with.```
```

### Comparing `Gehu_erp-0.3/README.md` & `Gehu_erp-0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 ## Setup and Installation
 
 To use Gehu_erp, you need to install it via pip. First, ensure you have Python installed, then open a terminal and run the following command:
 
 ```
 pip install Gehu_erp
 ```
+## Docs
+
+For more information and examples, please visit the [documentation](https://gehu-erp.readthedocs.io/en/latest/index.html).
+
 
 ## Dependencies
 
 Gehu_erp depends on the following Python libraries:
 - requests
 - Pillow
 - beautifulsoup4
@@ -57,9 +61,8 @@
 ## Contributing
 
 If you would like to contribute to Gehu_erp, feel free to submit a pull request or open an issue on the GitHub repository.
 
 ## Acknowledgments
 
 - Thanks to the developers of `requests`, `Pillow`, and `beautifulsoup4` for their excellent libraries.
-- Special thanks to the developers and maintainers of the GEHU Student API for providing the API that this library interacts with.
-```
+- Special thanks to the developers and maintainers of the GEHU Student API for providing the API that this library interacts with.```
```

### Comparing `Gehu_erp-0.3/erp/util/headers.py` & `Gehu_erp-0.4/erp/util/headers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 SessionId=None
 RequestVerificationToken=None
 
 class ApisHeaders:
-    def __init__(self, data = None):
+    def __init__(self, data = None,type=None):
 
         headers = {
         
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/110.0",
         "Accept": "*/*",
         "Accept-Language": "en-US,en;q=0.5",
         "Accept-Encoding": "gzip, deflate, br",
@@ -16,15 +16,17 @@
         "Sec-Fetch-Dest": "empty",
         "Sec-Fetch-Mode": "cors",
         "Sec-Fetch-Site": "same-origin",
         }
         if SessionId:
             headers["Cookie"]=f"ASP.NET_SessionId={SessionId}; __RequestVerificationToken={RequestVerificationToken}"
         if data:
-            headers["Content-Type"]="application/x-www-form-urlencoded"
+            if not type:
+                type="application/x-www-form-urlencoded"
+            headers["Content-Type"]=type
             headers["Content-Length"]= f"{len(data)}"
 
         token_head = {
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
             "Accept-Encoding": "gzip, deflate, br",
             "Accept-Language": "en-GB,en-US;q=0.9,en;q=0.8",
             "Cache-Control": "max-age=0",
```

### Comparing `Gehu_erp-0.3/setup.py` & `Gehu_erp-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Gehu_erp",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     install_requires=[
         "requests",
         "Pillow",
         "beautifulsoup4"
     ],
     author="yato",
     description="A Python library for interacting with GEHU Student API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/aminobot22",
+    url="https://github.com/aminobot22/gehu_erp",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

