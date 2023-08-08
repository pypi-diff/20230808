# Comparing `tmp/Zxy_Private-0.0.1.tar.gz` & `tmp/Zxy_Private-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Zxy_Private-0.0.1.tar", last modified: Tue Aug  8 09:10:59 2023, max compression
+gzip compressed data, was "dist\Zxy_Private-0.0.2.tar", last modified: Tue Aug  8 13:30:46 2023, max compression
```

## Comparing `Zxy_Private-0.0.1.tar` & `Zxy_Private-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 09:10:59.000000 Zxy_Private-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-08-08 09:10:59.000000 Zxy_Private-0.0.1/OhMyChat_API/
--rw-rw-rw-   0        0        0     3935 2023-08-08 03:03:17.000000 Zxy_Private-0.0.1/OhMyChat_API/OhMyChat_API.py
--rw-rw-rw-   0        0        0      425 2023-08-08 08:52:23.000000 Zxy_Private-0.0.1/OhMyChat_API/__init__.py
--rw-rw-rw-   0        0        0      372 2023-08-08 09:10:59.000000 Zxy_Private-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-08 09:10:59.000000 Zxy_Private-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-08-08 09:10:48.000000 Zxy_Private-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-08 09:10:59.000000 Zxy_Private-0.0.1/Zxy_Private.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-08 09:10:59.000000 Zxy_Private-0.0.1/Zxy_Private.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      372 2023-08-08 09:10:59.000000 Zxy_Private-0.0.1/Zxy_Private.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-08-08 09:10:59.000000 Zxy_Private-0.0.1/Zxy_Private.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2023-08-08 09:10:59.000000 Zxy_Private-0.0.1/Zxy_Private.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/OhMyChat_API/
+-rw-rw-rw-   0        0        0     3935 2023-08-08 03:03:17.000000 Zxy_Private-0.0.2/OhMyChat_API/Get_API.py
+-rw-rw-rw-   0        0        0      425 2023-08-08 08:52:23.000000 Zxy_Private-0.0.2/OhMyChat_API/__init__.py
+-rw-rw-rw-   0        0        0      366 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      470 2023-08-08 13:28:05.000000 Zxy_Private-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      366 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       13 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/top_level.txt
```

### Comparing `Zxy_Private-0.0.1/OhMyChat_API/OhMyChat_API.py` & `Zxy_Private-0.0.2/OhMyChat_API/Get_API.py`

 * *Files identical despite different names*

