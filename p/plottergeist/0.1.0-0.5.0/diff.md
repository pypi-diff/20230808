# Comparing `tmp/plottergeist-0.1.0.tar.gz` & `tmp/plottergeist-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plottergeist-0.1.0.tar", last modified: Fri Jul  7 22:54:22 2023, max compression
+gzip compressed data, was "dist/plottergeist-0.5.0.tar", last modified: Tue Aug  8 15:59:30 2023, max compression
```

## Comparing `plottergeist-0.1.0.tar` & `plottergeist-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-07-07 22:54:22.600009 plottergeist-0.1.0/
--rw-r--r--   0 apereiro   (501) staff       (20)     1066 2023-07-06 15:44:15.000000 plottergeist-0.1.0/LICENSE
--rw-r--r--   0 apereiro   (501) staff       (20)      399 2023-07-07 22:54:22.599825 plottergeist-0.1.0/PKG-INFO
--rw-r--r--   0 apereiro   (501) staff       (20)       14 2023-07-06 15:44:15.000000 plottergeist-0.1.0/README.md
-drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-07-07 22:54:22.598858 plottergeist-0.1.0/plottergeist/
--rw-r--r--   0 apereiro   (501) staff       (20)     2029 2023-07-06 16:41:25.000000 plottergeist-0.1.0/plottergeist/histogram.py
-drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-07-07 22:54:22.599651 plottergeist-0.1.0/plottergeist.egg-info/
--rw-r--r--   0 apereiro   (501) staff       (20)      399 2023-07-07 22:54:22.000000 plottergeist-0.1.0/plottergeist.egg-info/PKG-INFO
--rw-r--r--   0 apereiro   (501) staff       (20)      231 2023-07-07 22:54:22.000000 plottergeist-0.1.0/plottergeist.egg-info/SOURCES.txt
--rw-r--r--   0 apereiro   (501) staff       (20)        1 2023-07-07 22:54:22.000000 plottergeist-0.1.0/plottergeist.egg-info/dependency_links.txt
--rw-r--r--   0 apereiro   (501) staff       (20)       23 2023-07-07 22:54:22.000000 plottergeist-0.1.0/plottergeist.egg-info/requires.txt
--rw-r--r--   0 apereiro   (501) staff       (20)       13 2023-07-07 22:54:22.000000 plottergeist-0.1.0/plottergeist.egg-info/top_level.txt
--rw-r--r--   0 apereiro   (501) staff       (20)       38 2023-07-07 22:54:22.600055 plottergeist-0.1.0/setup.cfg
--rw-r--r--   0 apereiro   (501) staff       (20)      921 2023-07-07 22:50:05.000000 plottergeist-0.1.0/setup.py
+drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 15:59:30.382806 plottergeist-0.5.0/
+-rw-r--r--   0 apereiro   (501) staff       (20)     1066 2023-07-06 15:44:15.000000 plottergeist-0.5.0/LICENSE
+-rw-r--r--   0 apereiro   (501) staff       (20)      713 2023-08-08 15:59:30.382673 plottergeist-0.5.0/PKG-INFO
+-rw-r--r--   0 apereiro   (501) staff       (20)      329 2023-07-10 14:41:16.000000 plottergeist-0.5.0/README.md
+drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 15:59:30.380197 plottergeist-0.5.0/plottergeist/
+-rw-r--r--   0 apereiro   (501) staff       (20)      140 2023-07-10 14:49:21.000000 plottergeist-0.5.0/plottergeist/__init__.py
+-rw-r--r--   0 apereiro   (501) staff       (20)    13337 2023-07-11 11:00:32.000000 plottergeist-0.5.0/plottergeist/fig_creator.py
+-rw-r--r--   0 apereiro   (501) staff       (20)     2029 2023-07-09 10:54:33.000000 plottergeist-0.5.0/plottergeist/histogram.py
+-rw-r--r--   0 apereiro   (501) staff       (20)     1870 2023-07-10 14:41:16.000000 plottergeist-0.5.0/plottergeist/residuals.py
+-rw-r--r--   0 apereiro   (501) staff       (20)    36435 2023-07-11 10:33:05.000000 plottergeist-0.5.0/plottergeist/style.py
+drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 15:59:30.381643 plottergeist-0.5.0/plottergeist.egg-info/
+-rw-r--r--   0 apereiro   (501) staff       (20)      713 2023-08-08 15:59:30.000000 plottergeist-0.5.0/plottergeist.egg-info/PKG-INFO
+-rw-r--r--   0 apereiro   (501) staff       (20)      397 2023-08-08 15:59:30.000000 plottergeist-0.5.0/plottergeist.egg-info/SOURCES.txt
+-rw-r--r--   0 apereiro   (501) staff       (20)        1 2023-08-08 15:59:30.000000 plottergeist-0.5.0/plottergeist.egg-info/dependency_links.txt
+-rw-r--r--   0 apereiro   (501) staff       (20)       23 2023-08-08 15:59:30.000000 plottergeist-0.5.0/plottergeist.egg-info/requires.txt
+-rw-r--r--   0 apereiro   (501) staff       (20)       13 2023-08-08 15:59:30.000000 plottergeist-0.5.0/plottergeist.egg-info/top_level.txt
+-rw-r--r--   0 apereiro   (501) staff       (20)       38 2023-08-08 15:59:30.382863 plottergeist-0.5.0/setup.cfg
+-rw-r--r--   0 apereiro   (501) staff       (20)      921 2023-07-10 14:41:16.000000 plottergeist-0.5.0/setup.py
+drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 15:59:30.382340 plottergeist-0.5.0/test/
+-rw-r--r--   0 apereiro   (501) staff       (20)      450 2023-07-09 11:49:36.000000 plottergeist-0.5.0/test/test_histogram.py
+-rw-r--r--   0 apereiro   (501) staff       (20)     4047 2023-07-11 15:07:52.000000 plottergeist-0.5.0/test/test_plot_1D.py
+-rw-r--r--   0 apereiro   (501) staff       (20)     2660 2023-07-11 10:18:24.000000 plottergeist-0.5.0/test/test_plot_3D.py
```

### Comparing `plottergeist-0.1.0/LICENSE` & `plottergeist-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plottergeist-0.1.0/plottergeist/histogram.py` & `plottergeist-0.5.0/plottergeist/histogram.py`

 * *Files identical despite different names*

### Comparing `plottergeist-0.1.0/setup.py` & `plottergeist-0.5.0/setup.py`

 * *Files identical despite different names*

