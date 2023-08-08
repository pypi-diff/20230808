# Comparing `tmp/autorunpy-7.0.0.tar.gz` & `tmp/autorunpy-7.1.0.tar.gz`

## Comparing `autorunpy-7.0.0.tar` & `autorunpy-7.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-7.0.0/.github/workflows/publish-on-pip-on-release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/ret_module_2_run.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/ret_pkg_name.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/rm_venv.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/util.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 autorunpy-7.0.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-7.0.0/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-7.0.0/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-7.1.0/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-7.1.0/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 autorunpy-7.1.0/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 autorunpy-7.1.0/src/autorunpy/ret_module_2_run.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autorunpy-7.1.0/src/autorunpy/ret_pkg_name.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 autorunpy-7.1.0/src/autorunpy/rm_venv.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 autorunpy-7.1.0/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 autorunpy-7.1.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-7.1.0/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-7.1.0/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-7.1.0/PKG-INFO
```

### Comparing `autorunpy-7.0.0/.github/workflows/publish-on-pip-on-release.yml` & `autorunpy-7.1.0/.github/workflows/publish-on-pip-on-release.yml`

 * *Files identical despite different names*

### Comparing `autorunpy-7.0.0/src/autorunpy/make_venv.py` & `autorunpy-7.1.0/src/autorunpy/make_venv.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 from .util import Conf
 from .util import read_json
 
 c = Conf()
 
 def make_venv(fp) :
-    """ make virtualenv with pyenv, delete existing venv if it exists"""
+    """ make virtualenv with pyenv, delete existing venv if it exists """
     j = read_json(fp)
 
     py_ver = j[c.py_ver]
     pkg = j[c.pkg]
 
     venv_name = pkg + py_ver
 
     subprocess.run(['pyenv' , 'install' , '--skip-existing' , py_ver])
-    subprocess.run(['pyenv' , 'virtualenv' , py_ver , venv_name])
+    subprocess.run(['pyenv' , 'virtualenv' , py_ver , venv_name , ' &> n.out'])
 
     print(venv_name)
 
 if __name__ == '__main__' :
     conf_fn = sys.argv[1]
     make_venv(conf_fn)
```

### Comparing `autorunpy-7.0.0/.gitignore` & `autorunpy-7.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-7.0.0/LICENSE` & `autorunpy-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-7.0.0/PKG-INFO` & `autorunpy-7.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autorunpy
-Version: 7.0.0
+Version: 7.1.0
 Summary: Tools for auto running python scripts
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

