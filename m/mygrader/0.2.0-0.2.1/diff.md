# Comparing `tmp/mygrader-0.2.0.tar.gz` & `tmp/mygrader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mygrader-0.2.0.tar", last modified: Mon Aug  7 17:17:48 2023, max compression
+gzip compressed data, was "mygrader-0.2.1.tar", last modified: Tue Aug  8 05:45:00 2023, max compression
```

## Comparing `mygrader-0.2.0.tar` & `mygrader-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.621251 mygrader-0.2.0/
--rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.2.0/LICENSE
--rw-r--r--   0 iccie      (501) staff       (20)     2753 2023-08-07 17:17:48.621074 mygrader-0.2.0/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.2.0/README.md
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.614435 mygrader-0.2.0/mygrader.egg-info/
--rw-r--r--   0 iccie      (501) staff       (20)     2753 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)      889 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/SOURCES.txt
--rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/dependency_links.txt
--rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/entry_points.txt
--rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/requires.txt
--rw-r--r--   0 iccie      (501) staff       (20)        4 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/top_level.txt
--rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-07 17:17:48.621906 mygrader-0.2.0/setup.cfg
--rw-r--r--   0 iccie      (501) staff       (20)     1155 2023-08-07 17:17:44.000000 mygrader-0.2.0/setup.py
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.614558 mygrader-0.2.0/src/
--rw-r--r--   0 iccie      (501) staff       (20)        0 2023-08-07 05:56:28.000000 mygrader-0.2.0/src/__init__.py
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.615254 mygrader-0.2.0/src/mygrader/
--rw-r--r--   0 iccie      (501) staff       (20)       87 2023-08-07 05:56:21.000000 mygrader-0.2.0/src/mygrader/__init__.py
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.616090 mygrader-0.2.0/src/mygrader/cs111/
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.619915 mygrader-0.2.0/src/mygrader/cs111/CS66/
--rw-r--r--   0 iccie      (501) staff       (20)      565 2023-08-07 17:12:38.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/__init__.py
--rw-r--r--   0 iccie      (501) staff       (20)     2294 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/base_b.py
--rw-r--r--   0 iccie      (501) staff       (20)      832 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/corner_frame.py
--rw-r--r--   0 iccie      (501) staff       (20)     1609 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/dest_rotate_list.py
--rw-r--r--   0 iccie      (501) staff       (20)     1985 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/medal_allocation.py
--rw-r--r--   0 iccie      (501) staff       (20)     1848 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/moving_average.py
--rw-r--r--   0 iccie      (501) staff       (20)     4375 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/num_to_word.py
--rw-r--r--   0 iccie      (501) staff       (20)     1551 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/pi.py
--rw-r--r--   0 iccie      (501) staff       (20)     1575 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/print_polynomial.py
--rw-r--r--   0 iccie      (501) staff       (20)     1371 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/recursion_gcd.py
--rw-r--r--   0 iccie      (501) staff       (20)     1293 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/reverse_digits.py
--rw-r--r--   0 iccie      (501) staff       (20)     1853 2023-08-07 17:00:24.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/substitute_once.py
--rw-r--r--   0 iccie      (501) staff       (20)      623 2023-08-07 17:00:24.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/triangle.py
--rw-r--r--   0 iccie      (501) staff       (20)      722 2023-08-07 17:00:24.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/uniform.py
--rw-r--r--   0 iccie      (501) staff       (20)        0 2023-08-07 16:52:13.000000 mygrader-0.2.0/src/mygrader/cs111/__init__.py
--rw-r--r--   0 iccie      (501) staff       (20)     1493 2023-08-07 05:22:22.000000 mygrader-0.2.0/src/mygrader/printer.py
--rw-r--r--   0 iccie      (501) staff       (20)      560 2023-08-06 20:09:42.000000 mygrader-0.2.0/src/mygrader/writer.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-08 05:45:00.226142 mygrader-0.2.1/
+-rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.2.1/LICENSE
+-rw-r--r--   0 iccie      (501) staff       (20)     2753 2023-08-08 05:45:00.225983 mygrader-0.2.1/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.2.1/README.md
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-08 05:45:00.217719 mygrader-0.2.1/mygrader.egg-info/
+-rw-r--r--   0 iccie      (501) staff       (20)     2753 2023-08-08 05:45:00.000000 mygrader-0.2.1/mygrader.egg-info/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)      889 2023-08-08 05:45:00.000000 mygrader-0.2.1/mygrader.egg-info/SOURCES.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-08 05:45:00.000000 mygrader-0.2.1/mygrader.egg-info/dependency_links.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-08 05:45:00.000000 mygrader-0.2.1/mygrader.egg-info/entry_points.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-08 05:45:00.000000 mygrader-0.2.1/mygrader.egg-info/requires.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        4 2023-08-08 05:45:00.000000 mygrader-0.2.1/mygrader.egg-info/top_level.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-08 05:45:00.226188 mygrader-0.2.1/setup.cfg
+-rw-r--r--   0 iccie      (501) staff       (20)     1155 2023-08-08 05:44:58.000000 mygrader-0.2.1/setup.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-08 05:45:00.217857 mygrader-0.2.1/src/
+-rw-r--r--   0 iccie      (501) staff       (20)        0 2023-08-07 05:56:28.000000 mygrader-0.2.1/src/__init__.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-08 05:45:00.221886 mygrader-0.2.1/src/mygrader/
+-rw-r--r--   0 iccie      (501) staff       (20)       87 2023-08-07 05:56:21.000000 mygrader-0.2.1/src/mygrader/__init__.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-08 05:45:00.222294 mygrader-0.2.1/src/mygrader/cs111/
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-08 05:45:00.225715 mygrader-0.2.1/src/mygrader/cs111/CS66/
+-rw-r--r--   0 iccie      (501) staff       (20)      565 2023-08-07 17:12:38.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/__init__.py
+-rw-r--r--   0 iccie      (501) staff       (20)     2294 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/base_b.py
+-rw-r--r--   0 iccie      (501) staff       (20)      832 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/corner_frame.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1609 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/dest_rotate_list.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1985 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/medal_allocation.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1848 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/moving_average.py
+-rw-r--r--   0 iccie      (501) staff       (20)     4375 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/num_to_word.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1551 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/pi.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1575 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/print_polynomial.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1371 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/recursion_gcd.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1293 2023-08-07 16:59:35.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/reverse_digits.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1853 2023-08-07 17:00:24.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/substitute_once.py
+-rw-r--r--   0 iccie      (501) staff       (20)      623 2023-08-07 17:00:24.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/triangle.py
+-rw-r--r--   0 iccie      (501) staff       (20)      722 2023-08-07 17:00:24.000000 mygrader-0.2.1/src/mygrader/cs111/CS66/uniform.py
+-rw-r--r--   0 iccie      (501) staff       (20)        0 2023-08-07 16:52:13.000000 mygrader-0.2.1/src/mygrader/cs111/__init__.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1236 2023-08-08 05:43:10.000000 mygrader-0.2.1/src/mygrader/printer.py
+-rw-r--r--   0 iccie      (501) staff       (20)      560 2023-08-06 20:09:42.000000 mygrader-0.2.1/src/mygrader/writer.py
```

### Comparing `mygrader-0.2.0/LICENSE` & `mygrader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/PKG-INFO` & `mygrader-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mygrader
-Version: 0.2.0
+Version: 0.2.1
 Summary: my own CS111 grader.
 Home-page: https://github.com/AppleBoiy/my-grader
 Author: AppleBoiy
 Author-email: contact.chaipat@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mygrader-0.2.0/README.md` & `mygrader-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/mygrader.egg-info/PKG-INFO` & `mygrader-0.2.1/mygrader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mygrader
-Version: 0.2.0
+Version: 0.2.1
 Summary: my own CS111 grader.
 Home-page: https://github.com/AppleBoiy/my-grader
 Author: AppleBoiy
 Author-email: contact.chaipat@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mygrader-0.2.0/mygrader.egg-info/SOURCES.txt` & `mygrader-0.2.1/mygrader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/setup.py` & `mygrader-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mygrader',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[],  # Add any required dependencies here
     author='AppleBoiy',
 
     author_email='contact.chaipat@gmail.com',
     description='my own CS111 grader.',
     long_description=long_description,
```

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/__init__.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/__init__.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/base_b.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/base_b.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/corner_frame.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/corner_frame.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/dest_rotate_list.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/dest_rotate_list.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/medal_allocation.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/medal_allocation.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/moving_average.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/moving_average.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/num_to_word.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/num_to_word.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/pi.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/pi.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/print_polynomial.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/print_polynomial.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/recursion_gcd.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/recursion_gcd.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/reverse_digits.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/reverse_digits.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/substitute_once.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/substitute_once.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/triangle.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/triangle.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/cs111/CS66/uniform.py` & `mygrader-0.2.1/src/mygrader/cs111/CS66/uniform.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.2.0/src/mygrader/printer.py` & `mygrader-0.2.1/src/mygrader/printer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,39 @@
+from typing import List, Tuple
 
-def print_test_results(num_passed, num_failed, failed_cases):
+from .writer import write_failed_cases_to_file
+
+
+def print_test_results(num_passed: int, num_failed: int, failed_cases: List[Tuple], write_on_file: bool = False):
     """
     Print the test results and return the list of failed cases.
 
     Parameters:
-        num_passed (int): Number of test cases passed.
-        num_failed (int): Number of test cases failed.
-        failed_cases (list): List of tuples containing failed test cases.
+        :param num_passed: Number of test cases passed.
+        :param num_failed: Number of test cases failed.
+        :param failed_cases: List of tuples containing failed test cases.
+        :param write_on_file:
 
     Returns:
         list: List of dictionaries containing failed test cases.
 
     """
     print(f"{num_passed} test cases passed.")
 
+    failed_cases_list = []
 
     if num_failed > 0:
         print(f"{num_failed} test cases failed.")
 
         for i, failed_case in enumerate(failed_cases, start=1):
-            if i > 10:
-                break
+            if i < 10:
+                print(f"{i}. Input: {failed_case[0]}, Expected: {failed_case[1]}, Got: {failed_case[2]}")
+            failed_cases_list.append(
+                {"Input": failed_cases[i][0], "Expected": failed_case[i][1], "Got": failed_cases[i][2]}
+            )
+
+        if write_on_file:
+            write_failed_cases_to_file(failed_cases_list)
 
-            print(f"{i}. Input: {failed_case[0]}, Expected: {failed_case[1]}, Got: {failed_case[2]}")
 
     else:
         print("All test cases passed successfully.")
-
-    return [
-        {"Input": case[0], "Expected": case[1], "Got": case[2]} for case in failed_cases
-    ]
-
-
-def write_failed_cases_to_file(failed_cases, filename="failed_cases.txt"):
-    """
-    Write the list of failed cases to a file.
-
-    Parameters:
-        failed_cases (list): List of dictionaries containing failed test cases.
-        filename (str, optional): The name of the output file. Defaults to "failed_cases.txt".
-
-    """
-    with open(filename, "w") as file:
-        for i, failed_case in enumerate(failed_cases, start=1):
-            file.write(f"{i}. Input: {failed_case['Input']}, Expected: {failed_case['Expected']}, Got: {failed_case['Got']}\n")
```

### Comparing `mygrader-0.2.0/src/mygrader/writer.py` & `mygrader-0.2.1/src/mygrader/writer.py`

 * *Files identical despite different names*

