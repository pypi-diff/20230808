# Comparing `tmp/coopgame-0.8.tar.gz` & `tmp/coopgame-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\coopgame-0.8.tar", last modified: Thu Aug 20 18:28:59 2020, max compression
+gzip compressed data, was "dist\coopgame-0.9.tar", last modified: Fri Aug 21 17:49:13 2020, max compression
```

## Comparing `coopgame-0.8.tar` & `coopgame-0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2020-08-20 18:28:59.000000 coopgame-0.8/
--rw-rw-rw-   0        0        0     2237 2020-08-20 18:28:59.000000 coopgame-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1120 2020-07-29 02:56:04.000000 coopgame-0.8/README.md
-drwxrwxrwx   0        0        0        0 2020-08-20 18:28:59.000000 coopgame-0.8/coopgame/
--rw-rw-rw-   0        0        0        0 2020-07-29 03:05:48.000000 coopgame-0.8/coopgame/__init__.py
--rw-rw-rw-   0        0        0      457 2020-08-19 15:32:50.000000 coopgame-0.8/coopgame/colors.py
--rw-rw-rw-   0        0        0    12899 2020-08-19 03:05:30.000000 coopgame-0.8/coopgame/curves.py
--rw-rw-rw-   0        0        0     1255 2020-08-03 05:01:13.000000 coopgame-0.8/coopgame/enums.py
--rw-rw-rw-   0        0        0     8761 2020-08-19 19:33:48.000000 coopgame-0.8/coopgame/gameTemplate.py
--rw-rw-rw-   0        0        0     3659 2020-08-19 21:22:02.000000 coopgame-0.8/coopgame/pygamehelpers.py
--rw-rw-rw-   0        0        0    14676 2020-07-28 21:58:01.000000 coopgame-0.8/coopgame/pygbutton.py
--rw-rw-rw-   0        0        0     2660 2020-08-19 21:22:53.000000 coopgame-0.8/coopgame/pygraphhandler.py
--rw-rw-rw-   0        0        0    12417 2020-08-19 21:22:02.000000 coopgame-0.8/coopgame/pygridhandler.py
--rw-rw-rw-   0        0        0     3174 2020-08-20 18:26:09.000000 coopgame-0.8/coopgame/sprites.py
--rw-rw-rw-   0        0        0     4826 2020-08-19 19:06:26.000000 coopgame-0.8/coopgame/spritesheet.py
-drwxrwxrwx   0        0        0        0 2020-08-20 18:28:59.000000 coopgame-0.8/coopgame.egg-info/
--rw-rw-rw-   0        0        0     2237 2020-08-20 18:28:59.000000 coopgame-0.8/coopgame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2020-08-20 18:28:59.000000 coopgame-0.8/coopgame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-08-20 18:28:59.000000 coopgame-0.8/coopgame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-07-29 02:36:52.000000 coopgame-0.8/coopgame.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      243 2020-08-20 18:28:59.000000 coopgame-0.8/coopgame.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2020-08-20 18:28:59.000000 coopgame-0.8/coopgame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-08-20 18:28:59.000000 coopgame-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1224 2020-08-20 18:28:55.000000 coopgame-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-08-21 17:49:13.000000 coopgame-0.9/
+-rw-rw-rw-   0        0        0     2237 2020-08-21 17:49:13.000000 coopgame-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1120 2020-07-29 02:56:04.000000 coopgame-0.9/README.md
+drwxrwxrwx   0        0        0        0 2020-08-21 17:49:13.000000 coopgame-0.9/coopgame/
+-rw-rw-rw-   0        0        0        0 2020-07-29 03:05:48.000000 coopgame-0.9/coopgame/__init__.py
+-rw-rw-rw-   0        0        0      457 2020-08-19 15:32:50.000000 coopgame-0.9/coopgame/colors.py
+-rw-rw-rw-   0        0        0    12899 2020-08-19 03:05:30.000000 coopgame-0.9/coopgame/curves.py
+-rw-rw-rw-   0        0        0     1255 2020-08-03 05:01:13.000000 coopgame-0.9/coopgame/enums.py
+-rw-rw-rw-   0        0        0     8761 2020-08-19 19:33:48.000000 coopgame-0.9/coopgame/gameTemplate.py
+-rw-rw-rw-   0        0        0     3659 2020-08-19 21:22:02.000000 coopgame-0.9/coopgame/pygamehelpers.py
+-rw-rw-rw-   0        0        0    14676 2020-07-28 21:58:01.000000 coopgame-0.9/coopgame/pygbutton.py
+-rw-rw-rw-   0        0        0     2660 2020-08-19 21:22:53.000000 coopgame-0.9/coopgame/pygraphhandler.py
+-rw-rw-rw-   0        0        0    12417 2020-08-19 21:22:02.000000 coopgame-0.9/coopgame/pygridhandler.py
+-rw-rw-rw-   0        0        0     3139 2020-08-20 21:41:29.000000 coopgame-0.9/coopgame/sprites.py
+-rw-rw-rw-   0        0        0     6992 2020-08-21 17:33:07.000000 coopgame-0.9/coopgame/spritesheet.py
+drwxrwxrwx   0        0        0        0 2020-08-21 17:49:13.000000 coopgame-0.9/coopgame.egg-info/
+-rw-rw-rw-   0        0        0     2237 2020-08-21 17:49:13.000000 coopgame-0.9/coopgame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2020-08-21 17:49:13.000000 coopgame-0.9/coopgame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-08-21 17:49:13.000000 coopgame-0.9/coopgame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-07-29 02:36:52.000000 coopgame-0.9/coopgame.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      243 2020-08-21 17:49:13.000000 coopgame-0.9/coopgame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2020-08-21 17:49:13.000000 coopgame-0.9/coopgame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-08-21 17:49:13.000000 coopgame-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2020-08-21 17:49:08.000000 coopgame-0.9/setup.py
```

### Comparing `coopgame-0.8/PKG-INFO` & `coopgame-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopgame
-Version: 0.8
+Version: 0.9
 Summary: Tooling and templates used for building games
 Home-page: https://github.com/tylertjburns/coopgame
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Description: # coopgame
         Library of tooling and templates used for building games
```

### Comparing `coopgame-0.8/README.md` & `coopgame-0.9/README.md`

 * *Files identical despite different names*

### Comparing `coopgame-0.8/coopgame/curves.py` & `coopgame-0.9/coopgame/curves.py`

 * *Files identical despite different names*

### Comparing `coopgame-0.8/coopgame/enums.py` & `coopgame-0.9/coopgame/enums.py`

 * *Files identical despite different names*

### Comparing `coopgame-0.8/coopgame/gameTemplate.py` & `coopgame-0.9/coopgame/gameTemplate.py`

 * *Files identical despite different names*

### Comparing `coopgame-0.8/coopgame/pygamehelpers.py` & `coopgame-0.9/coopgame/pygamehelpers.py`

 * *Files identical despite different names*

### Comparing `coopgame-0.8/coopgame/pygbutton.py` & `coopgame-0.9/coopgame/pygbutton.py`

 * *Files identical despite different names*

### Comparing `coopgame-0.8/coopgame/pygraphhandler.py` & `coopgame-0.9/coopgame/pygraphhandler.py`

 * *Files identical despite different names*

### Comparing `coopgame-0.8/coopgame/pygridhandler.py` & `coopgame-0.9/coopgame/pygridhandler.py`

 * *Files identical despite different names*

### Comparing `coopgame-0.8/coopgame/sprites.py` & `coopgame-0.9/coopgame/sprites.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 
         self.image = None
         self._set_image()
 
     def set_animation(self, animation: str):
         if animation in self._animation_dict.keys():
             self._animation_key = animation
-        self._animation_index = 0
 
     def increment_animation_phase(self):
         self._animation_index += 1
         if self._animation_index >= len(self._animation_dict[self._animation_key]):
             self._animation_index = 0
 
         self._set_image()
```

### Comparing `coopgame-0.8/coopgame.egg-info/PKG-INFO` & `coopgame-0.9/coopgame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopgame
-Version: 0.8
+Version: 0.9
 Summary: Tooling and templates used for building games
 Home-page: https://github.com/tylertjburns/coopgame
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Description: # coopgame
         Library of tooling and templates used for building games
```

### Comparing `coopgame-0.8/setup.py` & `coopgame-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='coopgame',
-      version='0.8',
+      version='0.9',
       description='Tooling and templates used for building games',
       url='https://github.com/tylertjburns/coopgame',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.5",
```

