# Comparing `tmp/passwordless-27-0.0.1.tar.gz` & `tmp/passwordless_27-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-27-0.0.1.tar", last modified: Tue Aug  1 22:28:41 2023, max compression
+gzip compressed data, was "passwordless_27-0.1.1.tar", last modified: Tue Aug  8 06:37:54 2023, max compression
```

## Comparing `passwordless-27-0.0.1.tar` & `passwordless_27-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:28:41.137658 passwordless-27-0.0.1/
--rw-rw-rw-   0        0        0      481 2023-08-01 22:28:41.137658 passwordless-27-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 22:28:41.137151 passwordless-27-0.0.1/passwordless_27.egg-info/
--rw-rw-rw-   0        0        0      481 2023-08-01 22:28:41.000000 passwordless-27-0.0.1/passwordless_27.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2023-08-01 22:28:41.000000 passwordless-27-0.0.1/passwordless_27.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:28:41.000000 passwordless-27-0.0.1/passwordless_27.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-01 22:28:41.000000 passwordless-27-0.0.1/passwordless_27.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 22:28:41.138164 passwordless-27-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-08-01 22:28:36.000000 passwordless-27-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:37:54.905260 passwordless_27-0.1.1/
+-rw-rw-rw-   0        0        0     3276 2023-08-08 06:37:54.904752 passwordless_27-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2023-08-07 09:51:26.000000 passwordless_27-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 06:37:54.889241 passwordless_27-0.1.1/passwordless-27/
+-rw-rw-rw-   0        0        0       38 2023-08-07 09:46:22.000000 passwordless_27-0.1.1/passwordless-27/__init__.py
+-rw-rw-rw-   0        0        0     2256 2023-08-07 09:32:02.000000 passwordless_27-0.1.1/passwordless-27/client.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:37:54.904229 passwordless_27-0.1.1/passwordless_27.egg-info/
+-rw-rw-rw-   0        0        0     3276 2023-08-08 06:37:54.000000 passwordless_27-0.1.1/passwordless_27.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-08-08 06:37:54.000000 passwordless_27-0.1.1/passwordless_27.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 06:37:54.000000 passwordless_27-0.1.1/passwordless_27.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 06:37:54.000000 passwordless_27-0.1.1/passwordless_27.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-08 06:37:54.000000 passwordless_27-0.1.1/passwordless_27.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 06:37:54.905260 passwordless_27-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-08-07 09:46:17.000000 passwordless_27-0.1.1/setup.py
```

