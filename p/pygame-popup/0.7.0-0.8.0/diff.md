# Comparing `tmp/pygame-popup-0.7.0.tar.gz` & `tmp/pygame-popup-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame-popup-0.7.0.tar", last modified: Mon Aug  1 20:43:37 2022, max compression
+gzip compressed data, was "pygame-popup-0.8.0.tar", last modified: Tue Aug  8 16:04:54 2023, max compression
```

## Comparing `pygame-popup-0.7.0.tar` & `pygame-popup-0.8.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 20:43:37.152267 pygame-popup-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4584 2022-08-01 20:43:37.152267 pygame-popup-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4000 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-01 20:43:37.152267 pygame-popup-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 20:43:37.148266 pygame-popup-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 20:43:37.148266 pygame-popup-0.7.0/src/pygame_popup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4584 2022-08-01 20:43:37.000000 pygame-popup-0.7.0/src/pygame_popup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-08-01 20:43:37.000000 pygame-popup-0.7.0/src/pygame_popup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 20:43:37.000000 pygame-popup-0.7.0/src/pygame_popup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-01 20:43:37.000000 pygame-popup-0.7.0/src/pygame_popup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-01 20:43:37.000000 pygame-popup-0.7.0/src/pygame_popup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 20:43:37.148266 pygame-popup-0.7.0/src/pygamepopup/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 20:43:37.148266 pygame-popup-0.7.0/src/pygamepopup/_exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/_exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/_exceptions/wrong_initialization_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 20:43:37.148266 pygame-popup-0.7.0/src/pygamepopup/components/
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/components/box_element.py
--rw-r--r--   0 runner    (1001) docker     (121)     7807 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/components/button.py
--rw-r--r--   0 runner    (1001) docker     (121)     5931 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/components/dynamic_button.py
--rw-r--r--   0 runner    (1001) docker     (121)     6012 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/components/image_button.py
--rw-r--r--   0 runner    (1001) docker     (121)    14195 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/components/info_box.py
--rw-r--r--   0 runner    (1001) docker     (121)     4597 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/components/text_element.py
--rw-r--r--   0 runner    (1001) docker     (121)     4026 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 20:43:37.152267 pygame-popup-0.7.0/src/pygamepopup/images/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/images/default_box.png
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/images/default_box_hover.png
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/initialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/menu_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-08-01 20:43:33.000000 pygame-popup-0.7.0/src/pygamepopup/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:04:54.411219 pygame-popup-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-08 16:04:54.411219 pygame-popup-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 16:04:54.411219 pygame-popup-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:04:54.407218 pygame-popup-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:04:54.411219 pygame-popup-0.8.0/src/pygame_popup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-08 16:04:54.000000 pygame-popup-0.8.0/src/pygame_popup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-08 16:04:54.000000 pygame-popup-0.8.0/src/pygame_popup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:04:54.000000 pygame-popup-0.8.0/src/pygame_popup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 16:04:54.000000 pygame-popup-0.8.0/src/pygame_popup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 16:04:54.000000 pygame-popup-0.8.0/src/pygame_popup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:04:54.411219 pygame-popup-0.8.0/src/pygamepopup/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:04:54.411219 pygame-popup-0.8.0/src/pygamepopup/_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/_exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/_exceptions/wrong_initialization_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:04:54.411219 pygame-popup-0.8.0/src/pygamepopup/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/components/box_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/components/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/components/dynamic_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/components/image_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/components/info_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/components/text_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:04:54.411219 pygame-popup-0.8.0/src/pygamepopup/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/images/default_box.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/images/default_box_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/menu_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-08 16:04:49.000000 pygame-popup-0.8.0/src/pygamepopup/types.py
```

### Comparing `pygame-popup-0.7.0/LICENSE` & `pygame-popup-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/PKG-INFO` & `pygame-popup-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-popup
-Version: 0.7.0
+Version: 0.8.0
 Summary: A popup manager for pygame
 Home-page: https://github.com/Grimmys/pygame_popup_manager
 Author: Grimmys
 Author-email: grimmys.programming@gmail.com
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/Grimmys/pygame_popup_manager/issues
 Platform: UNKNOWN
```

### Comparing `pygame-popup-0.7.0/README.md` & `pygame-popup-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/setup.py` & `pygame-popup-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pygame-popup",
-    version="0.7.0",
+    version="0.8.0",
     author="Grimmys",
     author_email="grimmys.programming@gmail.com",
     description="A popup manager for pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Grimmys/pygame_popup_manager",
     project_urls={
```

### Comparing `pygame-popup-0.7.0/src/pygame_popup.egg-info/PKG-INFO` & `pygame-popup-0.8.0/src/pygame_popup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-popup
-Version: 0.7.0
+Version: 0.8.0
 Summary: A popup manager for pygame
 Home-page: https://github.com/Grimmys/pygame_popup_manager
 Author: Grimmys
 Author-email: grimmys.programming@gmail.com
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/Grimmys/pygame_popup_manager/issues
 Platform: UNKNOWN
```

### Comparing `pygame-popup-0.7.0/src/pygame_popup.egg-info/SOURCES.txt` & `pygame-popup-0.8.0/src/pygame_popup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/components/box_element.py` & `pygame-popup-0.8.0/src/pygamepopup/components/box_element.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/components/button.py` & `pygame-popup-0.8.0/src/pygamepopup/components/button.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/components/dynamic_button.py` & `pygame-popup-0.8.0/src/pygamepopup/components/dynamic_button.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/components/image_button.py` & `pygame-popup-0.8.0/src/pygamepopup/components/image_button.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/components/info_box.py` & `pygame-popup-0.8.0/src/pygamepopup/components/info_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         element_grid (list[list[BoxElement]]): a grid containing the components that should be rendered by the infoBox
         width (int): the width of the infoBox, defaults to DEFAULT_POPUP_WIDTH
         element_linked (pygame.Rect): the pygame Rect of the element linked to this infoBox,
             the infoBox will be displayed beside the element if provided
         has_close_button (bool): whether a close button should be added at the bottom or not, defaults to True
         title_color (pygame.Color): the color of the title
         background_path (str): the path corresponding to the image that should be the sprite of the infoBox
+        close_button_text (str): the text that will be shown on close button
         close_button_background_path (str): the path to the image corresponding to the sprite of the close button
             if there should be one
         close_button_background_hover_path (str): the path to the image corresponding to the sprite of
             the close button when it is hovered if there should be one
         visible_on_background (bool): whether the popup is visible on background or not, defaults to True
         has_vertical_separator (bool): whether there should be a line splitting the infoBox in two at middle width or
             not, defaults to False
@@ -76,14 +77,15 @@
         element_grid: list[list[BoxElement]],
         width: int = DEFAULT_POPUP_WIDTH,
         element_linked: pygame.Rect = None,
         position: Position = (0, 0),
         has_close_button: bool = True,
         title_color: pygame.Color = WHITE,
         background_path: str = None,
+        close_button_text: str = "Close",
         close_button_background_path: str = None,
         close_button_background_hover_path: str = None,
         visible_on_background: bool = True,
         has_vertical_separator: bool = False,
         identifier: str = "",
     ) -> None:
         self.title: str = title
@@ -98,14 +100,15 @@
         }
         background_path = (
             os.path.abspath(background_path)
             if background_path
             else _default_sprites["info_box_background"]
         )
         self.sprite: pygame.Surface = pygame.image.load(background_path)
+        self.close_button_text: str = close_button_text
         self.__close_button_background_path: str = close_button_background_path
         self.__close_button_background_hover_path: str = (
             close_button_background_hover_path
         )
         self.__elements: list[_Row] = self.init_elements()
         self.buttons: Sequence[Button] = []
         self.__size: tuple[int, int] = (width, 0)
@@ -166,15 +169,15 @@
         elements.insert(0, _Row([title]))
         if self.has_close_button:
             elements.append(
                 _Row(
                     [
                         Button(
                             size=CLOSE_BUTTON_SIZE,
-                            title="Close",
+                            title=self.close_button_text,
                             background_path=self.__close_button_background_path,
                             background_hover_path=self.__close_button_background_hover_path,
                             margin=(CLOSE_BUTTON_MARGIN_TOP, 0, 0, 0),
                         )
                     ]
                 )
             )
```

### Comparing `pygame-popup-0.7.0/src/pygamepopup/components/text_element.py` & `pygame-popup-0.8.0/src/pygamepopup/components/text_element.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/configuration.py` & `pygame-popup-0.8.0/src/pygamepopup/configuration.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/fonts.py` & `pygame-popup-0.8.0/src/pygamepopup/fonts.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/images/default_box.png` & `pygame-popup-0.8.0/src/pygamepopup/images/default_box.png`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/images/default_box_hover.png` & `pygame-popup-0.8.0/src/pygamepopup/images/default_box_hover.png`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/initialization.py` & `pygame-popup-0.8.0/src/pygamepopup/initialization.py`

 * *Files identical despite different names*

### Comparing `pygame-popup-0.7.0/src/pygamepopup/menu_manager.py` & `pygame-popup-0.8.0/src/pygamepopup/menu_manager.py`

 * *Files identical despite different names*

