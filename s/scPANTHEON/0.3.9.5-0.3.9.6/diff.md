# Comparing `tmp/scPANTHEON-0.3.9.5.tar.gz` & `tmp/scPANTHEON-0.3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scPANTHEON-0.3.9.5.tar", last modified: Tue Aug  8 06:36:33 2023, max compression
+gzip compressed data, was "dist\scPANTHEON-0.3.9.6.tar", last modified: Tue Aug  8 06:40:45 2023, max compression
```

## Comparing `scPANTHEON-0.3.9.5.tar` & `scPANTHEON-0.3.9.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.5/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      290 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.5/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scpantheon/app/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.5/scpantheon/app/__init__.py
--rw-rw-rw-   0        0        0     2607 2023-07-05 15:50:04.000000 scPANTHEON-0.3.9.5/scpantheon/app/bokeh_qt.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/scpantheon/front_end/
--rw-rw-rw-   0        0        0     6925 2023-08-08 06:35:36.000000 scPANTHEON-0.3.9.5/scpantheon/front_end/R_data_qt.py
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.5/scpantheon/front_end/__init__.py
--rw-rw-rw-   0        0        0     5711 2023-07-13 13:24:16.000000 scPANTHEON-0.3.9.5/scpantheon/front_end/data_qt.py
--rw-rw-rw-   0        0        0     3683 2023-07-10 13:33:19.000000 scPANTHEON-0.3.9.5/scpantheon/front_end/save_qt.py
--rw-rw-rw-   0        0        0     1363 2023-08-04 11:26:27.000000 scPANTHEON-0.3.9.5/scpantheon/main.py
--rw-rw-rw-   0        0        0    66286 2023-08-04 12:36:11.000000 scPANTHEON-0.3.9.5/scpantheon/source.py
--rw-rw-rw-   0        0        0       42 2023-08-08 06:36:33.000000 scPANTHEON-0.3.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1148 2023-08-08 06:36:22.000000 scPANTHEON-0.3.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      290 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.6/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scpantheon/app/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.6/scpantheon/app/__init__.py
+-rw-rw-rw-   0        0        0     2607 2023-07-05 15:50:04.000000 scPANTHEON-0.3.9.6/scpantheon/app/bokeh_qt.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/scpantheon/front_end/
+-rw-rw-rw-   0        0        0     6925 2023-08-08 06:35:36.000000 scPANTHEON-0.3.9.6/scpantheon/front_end/R_data_qt.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.6/scpantheon/front_end/__init__.py
+-rw-rw-rw-   0        0        0     5711 2023-07-13 13:24:16.000000 scPANTHEON-0.3.9.6/scpantheon/front_end/data_qt.py
+-rw-rw-rw-   0        0        0     3683 2023-07-10 13:33:19.000000 scPANTHEON-0.3.9.6/scpantheon/front_end/save_qt.py
+-rw-rw-rw-   0        0        0     1363 2023-08-04 11:26:27.000000 scPANTHEON-0.3.9.6/scpantheon/main.py
+-rw-rw-rw-   0        0        0    66286 2023-08-04 12:36:11.000000 scPANTHEON-0.3.9.6/scpantheon/source.py
+-rw-rw-rw-   0        0        0       42 2023-08-08 06:40:45.000000 scPANTHEON-0.3.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2023-08-08 06:40:32.000000 scPANTHEON-0.3.9.6/setup.py
```

### Comparing `scPANTHEON-0.3.9.5/scpantheon/app/bokeh_qt.py` & `scPANTHEON-0.3.9.6/scpantheon/app/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.5/scpantheon/front_end/R_data_qt.py` & `scPANTHEON-0.3.9.6/scpantheon/front_end/R_data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.5/scpantheon/front_end/data_qt.py` & `scPANTHEON-0.3.9.6/scpantheon/front_end/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.5/scpantheon/front_end/save_qt.py` & `scPANTHEON-0.3.9.6/scpantheon/front_end/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.5/scpantheon/main.py` & `scPANTHEON-0.3.9.6/scpantheon/main.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.5/scpantheon/source.py` & `scPANTHEON-0.3.9.6/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.9.5/setup.py` & `scPANTHEON-0.3.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.3.9.5',#版本
+    version='0.3.9.6',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon', 'scpantheon.app', 'scpantheon.front_end'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
                         'appdirs','rpy2'], # 依赖包,如果没有,可以不要
```

