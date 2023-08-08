# Comparing `tmp/excolor-0.0.3.tar.gz` & `tmp/excolor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excolor-0.0.3.tar", last modified: Mon Jul 31 17:56:13 2023, max compression
+gzip compressed data, was "excolor-0.0.4.tar", last modified: Tue Aug  8 15:00:03 2023, max compression
```

## Comparing `excolor-0.0.3.tar` & `excolor-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-31 17:56:13.230465 excolor-0.0.3/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2023-07-15 06:34:27.000000 excolor-0.0.3/LICENSE
--rw-r--r--   0 timpyrkov   (501) staff       (20)     3435 2023-07-31 17:56:13.230261 excolor-0.0.3/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)     2981 2023-07-31 17:52:37.000000 excolor-0.0.3/README.md
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-31 17:56:13.229477 excolor-0.0.3/excolor/
--rw-r--r--   0 timpyrkov   (501) staff       (20)      350 2023-07-25 04:09:40.000000 excolor-0.0.3/excolor/__init__.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)    12071 2023-07-25 21:36:31.000000 excolor-0.0.3/excolor/background.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)    12726 2023-07-25 19:44:55.000000 excolor-0.0.3/excolor/excolor.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)     2663 2023-07-25 12:27:34.000000 excolor-0.0.3/excolor/geometry.py
--rw-r--r--   0 timpyrkov   (501) staff       (20)     9404 2023-07-25 20:36:54.000000 excolor-0.0.3/excolor/imagetools.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)     9461 2023-07-25 04:17:01.000000 excolor-0.0.3/excolor/utils.py
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-31 17:56:13.230098 excolor-0.0.3/excolor.egg-info/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     3435 2023-07-31 17:56:12.000000 excolor-0.0.3/excolor.egg-info/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)      300 2023-07-31 17:56:13.000000 excolor-0.0.3/excolor.egg-info/SOURCES.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-31 17:56:12.000000 excolor-0.0.3/excolor.egg-info/dependency_links.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       61 2023-07-31 17:56:13.000000 excolor-0.0.3/excolor.egg-info/requires.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        8 2023-07-31 17:56:13.000000 excolor-0.0.3/excolor.egg-info/top_level.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-31 17:56:13.230546 excolor-0.0.3/setup.cfg
--rw-r--r--   0 timpyrkov   (501) staff       (20)      899 2023-07-31 17:54:34.000000 excolor-0.0.3/setup.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-08-08 15:00:03.369697 excolor-0.0.4/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2023-07-15 06:34:27.000000 excolor-0.0.4/LICENSE
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     3435 2023-08-08 15:00:03.369587 excolor-0.0.4/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     2981 2023-07-31 17:52:37.000000 excolor-0.0.4/README.md
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-08-08 15:00:03.368727 excolor-0.0.4/excolor/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      350 2023-07-25 04:09:40.000000 excolor-0.0.4/excolor/__init__.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)    12071 2023-07-25 21:36:31.000000 excolor-0.0.4/excolor/background.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)    12726 2023-07-25 19:44:55.000000 excolor-0.0.4/excolor/excolor.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)     2663 2023-07-25 12:27:34.000000 excolor-0.0.4/excolor/geometry.py
+-rw-r--r--   0 timpyrkov   (501) staff       (20)    10414 2023-08-08 14:56:44.000000 excolor-0.0.4/excolor/imagetools.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)     9461 2023-07-25 04:17:01.000000 excolor-0.0.4/excolor/utils.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-08-08 15:00:03.369409 excolor-0.0.4/excolor.egg-info/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     3435 2023-08-08 15:00:03.000000 excolor-0.0.4/excolor.egg-info/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      300 2023-08-08 15:00:03.000000 excolor-0.0.4/excolor.egg-info/SOURCES.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-08-08 15:00:03.000000 excolor-0.0.4/excolor.egg-info/dependency_links.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       61 2023-08-08 15:00:03.000000 excolor-0.0.4/excolor.egg-info/requires.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        8 2023-08-08 15:00:03.000000 excolor-0.0.4/excolor.egg-info/top_level.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-08-08 15:00:03.369734 excolor-0.0.4/setup.cfg
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      899 2023-08-08 14:57:31.000000 excolor-0.0.4/setup.py
```

### Comparing `excolor-0.0.3/LICENSE` & `excolor-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `excolor-0.0.3/PKG-INFO` & `excolor-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excolor
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extended colors for python
 Home-page: https://github.com/timpyrkov/excolor
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `excolor-0.0.3/README.md` & `excolor-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `excolor-0.0.3/excolor/background.py` & `excolor-0.0.4/excolor/background.py`

 * *Files identical despite different names*

### Comparing `excolor-0.0.3/excolor/excolor.py` & `excolor-0.0.4/excolor/excolor.py`

 * *Files identical despite different names*

### Comparing `excolor-0.0.3/excolor/geometry.py` & `excolor-0.0.4/excolor/geometry.py`

 * *Files identical despite different names*

### Comparing `excolor-0.0.3/excolor/imagetools.py` & `excolor-0.0.4/excolor/imagetools.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,68 @@
     plt.gca().set_axis_off()
     plt.subplots_adjust(top=1, bottom=0, right=1, left=0, hspace=0, wspace=0)
     plt.margins(0,0)
     plt.axis("off")
     return
 
 
+def to_prime_factors(n):
+    """
+    Utility function to split a number into prime factors
+    
+    Parameters
+    ----------
+    n : int
+        Width or height
+
+    Returns
+    -------
+    factors : list
+        Prime number factors
+
+    """
+    factors = []
+    i = 2
+    while i * i < n:
+        if n % i:
+            i += 1
+        else:
+            n //= i
+            factors.append(i)
+    factors.append(n)
+    factors.append(1)
+    return factors
+
+
+def size_to_size_and_dpi(size):
+    """
+    Splits image size (pixels) into size (~5 x 5 inches) and dpi
+    
+    Parameters
+    ----------
+    size : tuple
+        Width and height [pixels]
+
+    Returns
+    -------
+    size : tuple
+        Output image size [inches]
+    dpi : int
+        Output image resolution [dots per inch]
+
+    """
+    dpi = np.gcd(*size)
+    size = np.asarray(size) // dpi
+    dpi = to_prime_factors(dpi)
+    while size.min() < 5 and max(dpi) > 1:
+        size = dpi.pop(0) * size
+    dpi = np.prod(dpi)
+    return size, dpi
+
+
 def load_image(fname):
     """
     Converts image to numpy array
 
     Parameters
     ----------
     image : str
```

### Comparing `excolor-0.0.3/excolor/utils.py` & `excolor-0.0.4/excolor/utils.py`

 * *Files identical despite different names*

### Comparing `excolor-0.0.3/excolor.egg-info/PKG-INFO` & `excolor-0.0.4/excolor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excolor
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extended colors for python
 Home-page: https://github.com/timpyrkov/excolor
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `excolor-0.0.3/setup.py` & `excolor-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="excolor",
-    version="0.0.3",
+    version="0.0.4",
     author="Tim Pyrkov",
     author_email="tim.pyrkov@gmail.com",
     description="Extended colors for python",
     long_description=read("README.md"),
     license = "MIT License",
     long_description_content_type="text/markdown",
     url="https://github.com/timpyrkov/excolor",
```

