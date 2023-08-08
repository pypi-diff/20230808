# Comparing `tmp/todoist_auto-6.0.2.tar.gz` & `tmp/todoist_auto-6.0.3.tar.gz`

## Comparing `todoist_auto-6.0.2.tar` & `todoist_auto-6.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/__init__.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/models.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/rm_empty_sections.py
--rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/routine.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/util.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/LICENSE
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/README.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/pyproject.toml
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/src/todoist_auto/__init__.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/src/todoist_auto/models.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/src/todoist_auto/rm_empty_sections.py
+-rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/src/todoist_auto/routine.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/src/todoist_auto/util.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/LICENSE
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/README.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 todoist_auto-6.0.3/PKG-INFO
```

### Comparing `todoist_auto-6.0.2/.github/workflows/publish-on-pip.yml` & `todoist_auto-6.0.3/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.2/src/todoist_auto/models.py` & `todoist_auto-6.0.3/src/todoist_auto/models.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.2/src/todoist_auto/rm_empty_sections.py` & `todoist_auto-6.0.3/src/todoist_auto/rm_empty_sections.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
     ##
     # keep only routine project sections
     msk = dfs[ts.project_id].eq(pa.routine_proj_id)
     dfs = dfs[msk]
 
     ##
-    # split max time of sections from its name if exists
+    # split max time of section from its name if exists
     dfs = split_max_time_of_section_from_its_name(dfs)
 
     ##
     # find next reset datetime
     rrdt = find_next_reset_datetime()
 
     ##
@@ -161,7 +161,20 @@
 
 ##
 
 
 if __name__ == '__main__' :
     main()
     print(f'{Path(__file__).name} Done!')
+
+##
+
+if False :
+    pass
+
+    ##
+
+    ##
+
+    ##
+
+    ##
```

### Comparing `todoist_auto-6.0.2/src/todoist_auto/routine.py` & `todoist_auto-6.0.3/src/todoist_auto/routine.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.2/src/todoist_auto/util.py` & `todoist_auto-6.0.3/src/todoist_auto/util.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.2/.gitignore` & `todoist_auto-6.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.2/LICENSE` & `todoist_auto-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.2/PKG-INFO` & `todoist_auto-6.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todoist_auto
-Version: 6.0.2
+Version: 6.0.3
 Summary: Automating Todoist
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

