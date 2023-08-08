# Comparing `tmp/declination-1.0.tar.gz` & `tmp/declination-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declination-1.0.tar", last modified: Tue Aug  8 16:05:28 2023, max compression
+gzip compressed data, was "declination-1.0.1.tar", last modified: Tue Aug  8 16:37:56 2023, max compression
```

## Comparing `declination-1.0.tar` & `declination-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxr-xr-x   0 andrewhumphrey   (501) staff       (20)        0 2023-08-08 16:05:28.782056 declination-1.0/
--rw-r--r--   0 andrewhumphrey   (501) staff       (20)      490 2023-08-08 16:05:28.781824 declination-1.0/PKG-INFO
--rw-r--r--   0 andrewhumphrey   (501) staff       (20)      226 2023-08-08 15:36:57.000000 declination-1.0/README.txt
-drwxr-xr-x   0 andrewhumphrey   (501) staff       (20)        0 2023-08-08 16:05:28.781539 declination-1.0/declination.egg-info/
--rw-r--r--   0 andrewhumphrey   (501) staff       (20)      490 2023-08-08 16:05:28.000000 declination-1.0/declination.egg-info/PKG-INFO
--rw-r--r--   0 andrewhumphrey   (501) staff       (20)      174 2023-08-08 16:05:28.000000 declination-1.0/declination.egg-info/SOURCES.txt
--rw-r--r--   0 andrewhumphrey   (501) staff       (20)        1 2023-08-08 16:05:28.000000 declination-1.0/declination.egg-info/dependency_links.txt
--rw-r--r--   0 andrewhumphrey   (501) staff       (20)        1 2023-08-08 16:05:28.000000 declination-1.0/declination.egg-info/top_level.txt
--rw-r--r--   0 andrewhumphrey   (501) staff       (20)       87 2023-08-08 15:53:16.000000 declination-1.0/pyproject.toml
--rw-r--r--   0 andrewhumphrey   (501) staff       (20)       38 2023-08-08 16:05:28.782213 declination-1.0/setup.cfg
--rw-r--r--   0 andrewhumphrey   (501) staff       (20)      861 2023-08-08 16:05:11.000000 declination-1.0/setup.py
+drwxr-xr-x   0 andrewhumphrey   (501) staff       (20)        0 2023-08-08 16:37:56.581687 declination-1.0.1/
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)      492 2023-08-08 16:37:56.581491 declination-1.0.1/PKG-INFO
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)      226 2023-08-08 15:36:57.000000 declination-1.0.1/README.txt
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)       87 2023-08-08 15:53:16.000000 declination-1.0.1/pyproject.toml
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)       38 2023-08-08 16:37:56.581744 declination-1.0.1/setup.cfg
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)      760 2023-08-08 16:37:21.000000 declination-1.0.1/setup.py
+drwxr-xr-x   0 andrewhumphrey   (501) staff       (20)        0 2023-08-08 16:37:56.572911 declination-1.0.1/src/
+drwxr-xr-x   0 andrewhumphrey   (501) staff       (20)        0 2023-08-08 16:37:56.576568 declination-1.0.1/src/declination/
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)     1059 2023-08-08 16:22:29.000000 declination-1.0.1/src/declination/__init__.py
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)    11263 2023-08-08 15:35:40.000000 declination-1.0.1/src/declination/geomag.py
+drwxr-xr-x   0 andrewhumphrey   (501) staff       (20)        0 2023-08-08 16:37:56.579632 declination-1.0.1/src/declination.egg-info/
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)      492 2023-08-08 16:37:56.000000 declination-1.0.1/src/declination.egg-info/PKG-INFO
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)      270 2023-08-08 16:37:56.000000 declination-1.0.1/src/declination.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)        1 2023-08-08 16:37:56.000000 declination-1.0.1/src/declination.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)       12 2023-08-08 16:37:56.000000 declination-1.0.1/src/declination.egg-info/top_level.txt
+drwxr-xr-x   0 andrewhumphrey   (501) staff       (20)        0 2023-08-08 16:37:56.579796 declination-1.0.1/tests/
+-rw-r--r--   0 andrewhumphrey   (501) staff       (20)       31 2023-08-08 16:25:22.000000 declination-1.0.1/tests/test_declination.py
```

