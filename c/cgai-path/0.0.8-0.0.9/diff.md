# Comparing `tmp/cgai_path-0.0.8.tar.gz` & `tmp/cgai_path-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgai_path-0.0.8.tar", last modified: Wed Oct  5 16:42:49 2022, max compression
+gzip compressed data, was "cgai_path-0.0.9.tar", last modified: Tue Aug  8 07:13:56 2023, max compression
```

## Comparing `cgai_path-0.0.8.tar` & `cgai_path-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-10-05 16:42:49.442430 cgai_path-0.0.8/
--rw-rw-rw-   0        0        0    11558 2022-10-05 16:40:25.000000 cgai_path-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2002 2022-10-05 16:42:49.441430 cgai_path-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      814 2022-10-03 15:28:07.000000 cgai_path-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-05 16:42:49.423426 cgai_path-0.0.8/cgai_path/
--rw-rw-rw-   0        0        0     4764 2022-10-05 12:18:37.000000 cgai_path-0.0.8/cgai_path/Cpath.py
--rw-rw-rw-   0        0        0      261 2022-10-05 12:19:02.000000 cgai_path-0.0.8/cgai_path/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-05 16:42:49.437429 cgai_path-0.0.8/cgai_path.egg-info/
--rw-rw-rw-   0        0        0     2002 2022-10-05 16:42:49.000000 cgai_path-0.0.8/cgai_path.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2022-10-05 16:42:49.000000 cgai_path-0.0.8/cgai_path.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-05 16:42:49.000000 cgai_path-0.0.8/cgai_path.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-10-05 16:42:49.000000 cgai_path-0.0.8/cgai_path.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-05 16:42:49.442430 cgai_path-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1152 2022-10-05 12:19:07.000000 cgai_path-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:13:56.992051 cgai_path-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2022-10-05 16:40:25.000000 cgai_path-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1623 2023-08-08 07:13:56.992051 cgai_path-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      814 2022-10-03 15:28:07.000000 cgai_path-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 07:13:56.976036 cgai_path-0.0.9/cgai_path/
+-rw-rw-rw-   0        0        0      261 2023-08-08 07:11:25.000000 cgai_path-0.0.9/cgai_path/__init__.py
+-rw-rw-rw-   0        0        0     4764 2022-10-05 12:18:37.000000 cgai_path-0.0.9/cgai_path/cpath.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:13:56.987046 cgai_path-0.0.9/cgai_path.egg-info/
+-rw-rw-rw-   0        0        0     1623 2023-08-08 07:13:56.000000 cgai_path-0.0.9/cgai_path.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-08-08 07:13:56.000000 cgai_path-0.0.9/cgai_path.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 07:13:56.000000 cgai_path-0.0.9/cgai_path.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-08 07:13:56.000000 cgai_path-0.0.9/cgai_path.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 07:13:56.993052 cgai_path-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-08-08 07:11:18.000000 cgai_path-0.0.9/setup.py
```

### Comparing `cgai_path-0.0.8/LICENSE` & `cgai_path-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cgai_path-0.0.8/PKG-INFO` & `cgai_path-0.0.9/cgai_path.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 Metadata-Version: 2.1
-Name: cgai_path
-Version: 0.0.8
+Name: cgai-path
+Version: 0.0.9
 Summary: Easy operation of file path for CG industry.
 Home-page: https://github.com/zxzxde/cgai-path
 Author: Master Zhang
 Author-email: 360014296@qq.com
-License: UNKNOWN
-Description: #cgai-path
-        
-        
-        #### 功能
-        
-        应用于CG行业的文件路径
-        
-        
-        #### 基本使用
-        
-        ```python
-        import os
-        from cgai_path import CGAIPATH
-        
-        
-        
-        p = r'C:\PyOut\Test\test_hiero\v001\musk_%04d.exr'
-        
-        cpath = CGAIPATH()
-        
-        # 判断提供的路径是否为序列
-        result = cpath.isSequence(p)
-        print(result)  # ('C:\\PyOut\\Test\\test_hiero\\v001\\musk_', '%04d')
-        
-        if result:
-            filename = cpath.get_filename(p)
-            print(filename)  # musk
-        
-        # 获取文件序列
-        paths,missings = cpath.get_files(p)
-        print(paths) # ['C:\\PyOut\\Test\\test_hiero\\v001\\musk_0001.exr',...,'C:\\PyOut\\Test\\test_hiero\\v001\\musk_0049.exr']
-        print()
-        print(missings)
-        
-        
-        a = r'C:\PyOut\Test\test_hiero\v001\musk_0001.exr'
-        
-        # 获取文件名称
-        filename = cpath.get_filename(a)
-        print(filename)  # musk_0001
-        
-        
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+#cgai-path
+
+
+#### 功能
+
+应用于CG行业的文件路径
+
+
+#### 基本使用
+
+```python
+import os
+from cgai_path import CGAIPATH
+
+
+
+p = r'C:\PyOut\Test\test_hiero\v001\musk_%04d.exr'
+
+cpath = CGAIPATH()
+
+# 判断提供的路径是否为序列
+result = cpath.isSequence(p)
+print(result)  # ('C:\\PyOut\\Test\\test_hiero\\v001\\musk_', '%04d')
+
+if result:
+    filename = cpath.get_filename(p)
+    print(filename)  # musk
+
+# 获取文件序列
+paths,missings = cpath.get_files(p)
+print(paths) # ['C:\\PyOut\\Test\\test_hiero\\v001\\musk_0001.exr',...,'C:\\PyOut\\Test\\test_hiero\\v001\\musk_0049.exr']
+print()
+print(missings)
+
+
+a = r'C:\PyOut\Test\test_hiero\v001\musk_0001.exr'
+
+# 获取文件名称
+filename = cpath.get_filename(a)
+print(filename)  # musk_0001
+
+
+
+```
```

### Comparing `cgai_path-0.0.8/README.md` & `cgai_path-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cgai_path-0.0.8/cgai_path/Cpath.py` & `cgai_path-0.0.9/cgai_path/cpath.py`

 * *Files identical despite different names*

### Comparing `cgai_path-0.0.8/cgai_path.egg-info/PKG-INFO` & `cgai_path-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 Metadata-Version: 2.1
-Name: cgai-path
-Version: 0.0.8
+Name: cgai_path
+Version: 0.0.9
 Summary: Easy operation of file path for CG industry.
 Home-page: https://github.com/zxzxde/cgai-path
 Author: Master Zhang
 Author-email: 360014296@qq.com
-License: UNKNOWN
-Description: #cgai-path
-        
-        
-        #### 功能
-        
-        应用于CG行业的文件路径
-        
-        
-        #### 基本使用
-        
-        ```python
-        import os
-        from cgai_path import CGAIPATH
-        
-        
-        
-        p = r'C:\PyOut\Test\test_hiero\v001\musk_%04d.exr'
-        
-        cpath = CGAIPATH()
-        
-        # 判断提供的路径是否为序列
-        result = cpath.isSequence(p)
-        print(result)  # ('C:\\PyOut\\Test\\test_hiero\\v001\\musk_', '%04d')
-        
-        if result:
-            filename = cpath.get_filename(p)
-            print(filename)  # musk
-        
-        # 获取文件序列
-        paths,missings = cpath.get_files(p)
-        print(paths) # ['C:\\PyOut\\Test\\test_hiero\\v001\\musk_0001.exr',...,'C:\\PyOut\\Test\\test_hiero\\v001\\musk_0049.exr']
-        print()
-        print(missings)
-        
-        
-        a = r'C:\PyOut\Test\test_hiero\v001\musk_0001.exr'
-        
-        # 获取文件名称
-        filename = cpath.get_filename(a)
-        print(filename)  # musk_0001
-        
-        
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+#cgai-path
+
+
+#### 功能
+
+应用于CG行业的文件路径
+
+
+#### 基本使用
+
+```python
+import os
+from cgai_path import CGAIPATH
+
+
+
+p = r'C:\PyOut\Test\test_hiero\v001\musk_%04d.exr'
+
+cpath = CGAIPATH()
+
+# 判断提供的路径是否为序列
+result = cpath.isSequence(p)
+print(result)  # ('C:\\PyOut\\Test\\test_hiero\\v001\\musk_', '%04d')
+
+if result:
+    filename = cpath.get_filename(p)
+    print(filename)  # musk
+
+# 获取文件序列
+paths,missings = cpath.get_files(p)
+print(paths) # ['C:\\PyOut\\Test\\test_hiero\\v001\\musk_0001.exr',...,'C:\\PyOut\\Test\\test_hiero\\v001\\musk_0049.exr']
+print()
+print(missings)
+
+
+a = r'C:\PyOut\Test\test_hiero\v001\musk_0001.exr'
+
+# 获取文件名称
+filename = cpath.get_filename(a)
+print(filename)  # musk_0001
+
+
+
+```
```

### Comparing `cgai_path-0.0.8/setup.py` & `cgai_path-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="cgai_path",
-    version="0.0.8",
+    version="0.0.9",
     author="Master Zhang",
     author_email="360014296@qq.com",
     description="Easy operation of file path for CG industry.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zxzxde/cgai-path",
     packages=setuptools.find_packages(),
```

