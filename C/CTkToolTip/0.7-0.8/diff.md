# Comparing `tmp/CTkToolTip-0.7.tar.gz` & `tmp/CTkToolTip-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkToolTip-0.7.tar", last modified: Wed Aug  2 08:37:11 2023, max compression
+gzip compressed data, was "CTkToolTip-0.8.tar", last modified: Tue Aug  8 09:40:31 2023, max compression
```

## Comparing `CTkToolTip-0.7.tar` & `CTkToolTip-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:37:11.615525 CTkToolTip-0.7/
-drwxrwxrwx   0        0        0        0 2023-08-02 08:37:11.592204 CTkToolTip-0.7/CTkToolTip/
--rw-rw-rw-   0        0        0      225 2023-08-02 08:35:21.000000 CTkToolTip-0.7/CTkToolTip/__init__.py
--rw-rw-rw-   0        0        0     6727 2023-08-02 08:34:35.000000 CTkToolTip-0.7/CTkToolTip/ctk_tooltip.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:37:11.615525 CTkToolTip-0.7/CTkToolTip.egg-info/
--rw-rw-rw-   0        0        0     3673 2023-08-02 08:37:11.000000 CTkToolTip-0.7/CTkToolTip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-08-02 08:37:11.000000 CTkToolTip-0.7/CTkToolTip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:37:11.000000 CTkToolTip-0.7/CTkToolTip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-02 08:37:11.000000 CTkToolTip-0.7/CTkToolTip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkToolTip-0.7/LICENSE
--rw-rw-rw-   0        0        0     3673 2023-08-02 08:37:11.615525 CTkToolTip-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3011 2023-08-01 12:14:05.000000 CTkToolTip-0.7/README.md
--rw-rw-rw-   0        0        0      575 2023-08-02 08:37:11.622035 CTkToolTip-0.7/setup.cfg
--rw-rw-rw-   0        0        0      950 2023-08-02 08:36:32.000000 CTkToolTip-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:40:31.935654 CTkToolTip-0.8/
+drwxrwxrwx   0        0        0        0 2023-08-08 09:40:31.922009 CTkToolTip-0.8/CTkToolTip/
+-rw-rw-rw-   0        0        0      225 2023-08-08 09:33:42.000000 CTkToolTip-0.8/CTkToolTip/__init__.py
+-rw-rw-rw-   0        0        0     7453 2023-08-08 09:33:17.000000 CTkToolTip-0.8/CTkToolTip/ctk_tooltip.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:40:31.933654 CTkToolTip-0.8/CTkToolTip.egg-info/
+-rw-rw-rw-   0        0        0     3702 2023-08-08 09:40:31.000000 CTkToolTip-0.8/CTkToolTip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-08-08 09:40:31.000000 CTkToolTip-0.8/CTkToolTip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 09:40:31.000000 CTkToolTip-0.8/CTkToolTip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 09:40:31.000000 CTkToolTip-0.8/CTkToolTip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkToolTip-0.8/LICENSE
+-rw-rw-rw-   0        0        0     3702 2023-08-08 09:40:31.935654 CTkToolTip-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3039 2023-08-08 09:40:10.000000 CTkToolTip-0.8/README.md
+-rw-rw-rw-   0        0        0      575 2023-08-08 09:40:31.937656 CTkToolTip-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-08-08 09:34:29.000000 CTkToolTip-0.8/setup.py
```

### Comparing `CTkToolTip-0.7/CTkToolTip/ctk_tooltip.py` & `CTkToolTip-0.8/CTkToolTip/ctk_tooltip.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,144 +1,162 @@
 """
 CTkToolTip Widget
-version: 0.7
+version: 0.8
 """
 
 import time
 import sys
 import customtkinter
 from tkinter import Toplevel, Frame
 
 class CTkToolTip(Toplevel):
     """
     Creates a ToolTip (pop-up) widget for customtkinter.
     """
 
     def __init__(
-        self,
-        widget: any = None,
-        message: str = None,
-        delay: float = 0.2,
-        follow: bool = True,
-        x_offset: int = +20,
-        y_offset: int = +10,
-        bg_color: str = None,
-        corner_radius: int = 10,
-        border_width: int = 0,
-        border_color: str = None,
-        alpha: float = 0.8,
-        padding: tuple = (10,2),
-        **message_kwargs):
-        
+            self,
+            widget: any = None,
+            message: str = None,
+            delay: float = 0.2,
+            follow: bool = True,
+            x_offset: int = +20,
+            y_offset: int = +10,
+            bg_color: str = None,
+            corner_radius: int = 10,
+            border_width: int = 0,
+            border_color: str = None,
+            alpha: float = 0.95,
+            padding: tuple = (10, 2),
+            **message_kwargs):
+
         super().__init__()
 
         self.widget = widget
 
         self.withdraw()
-        
+
         # Disable ToolTip's title bar
         self.overrideredirect(True)
-                
+
         if sys.platform.startswith("win"):
-            self.transparent_color = self.widget._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkToplevel"]["fg_color"])
+            self.transparent_color = self.widget._apply_appearance_mode(
+                customtkinter.ThemeManager.theme["CTkToplevel"]["fg_color"])
             self.attributes("-transparentcolor", self.transparent_color)
             self.transient()
         elif sys.platform.startswith("darwin"):
             self.transparent_color = 'systemTransparent'
             self.attributes("-transparent", True)
             self.transient(self.master)
         else:
             self.transparent_color = '#000001'
             corner_radius = 0
             self.transient()
-            
+
         self.resizable(width=True, height=True)
-        
+
         # Make the background transparent
         self.config(background=self.transparent_color)
-        
+
         # StringVar instance for msg string
         self.messageVar = customtkinter.StringVar()
         self.message = message
         self.messageVar.set(self.message)
-      
+
         self.delay = delay
         self.follow = follow
         self.x_offset = x_offset
         self.y_offset = y_offset
         self.corner_radius = corner_radius
         self.alpha = alpha
         self.border_width = border_width
         self.padding = padding
         self.bg_color = customtkinter.ThemeManager.theme["CTkFrame"]["fg_color"] if bg_color is None else bg_color
         self.border_color = border_color
         self.disable = False
-        
+
         # visibility status of the ToolTip inside|outside|visible
         self.status = "outside"
         self.last_moved = 0
         self.attributes('-alpha', self.alpha)
 
         if sys.platform.startswith("win"):
-            if self.widget._apply_appearance_mode(self.bg_color)==self.transparent_color:
+            if self.widget._apply_appearance_mode(self.bg_color) == self.transparent_color:
                 self.transparent_color = "#000001"
                 self.config(background=self.transparent_color)
                 self.attributes("-transparentcolor", self.transparent_color)
-            
+
         # Add the message widget inside the tooltip
         self.transparent_frame = Frame(self, bg=self.transparent_color)
         self.transparent_frame.pack(padx=0, pady=0, fill="both", expand=True)
-        
-        self.frame = customtkinter.CTkFrame(self.transparent_frame, bg_color=self.transparent_color, corner_radius=self.corner_radius,
-                                            border_width=self.border_width, fg_color=self.bg_color, border_color=self.border_color)
+
+        self.frame = customtkinter.CTkFrame(self.transparent_frame, bg_color=self.transparent_color,
+                                            corner_radius=self.corner_radius,
+                                            border_width=self.border_width, fg_color=self.bg_color,
+                                            border_color=self.border_color)
         self.frame.pack(padx=0, pady=0, fill="both", expand=True)
-        
+
         self.message_label = customtkinter.CTkLabel(self.frame, textvariable=self.messageVar, **message_kwargs)
-        self.message_label.pack(fill="both", padx=self.padding[0]+self.border_width,
-                                pady=self.padding[1]+self.border_width, expand=True)
+        self.message_label.pack(fill="both", padx=self.padding[0] + self.border_width,
+                                pady=self.padding[1] + self.border_width, expand=True)
 
-        if self.widget.winfo_name()!="tk":
-            if self.frame.cget("fg_color")==self.widget.cget("bg_color"):
-                if not bg_color:             
-                    self._top_fg_color = self.frame._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"])
-                    if self._top_fg_color!=self.transparent_color:
+        if self.widget.winfo_name() != "tk":
+            if self.frame.cget("fg_color") == self.widget.cget("bg_color"):
+                if not bg_color:
+                    self._top_fg_color = self.frame._apply_appearance_mode(
+                        customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"])
+                    if self._top_fg_color != self.transparent_color:
                         self.frame.configure(fg_color=self._top_fg_color)
-        
+
         # Add bindings to the widget without overriding the existing ones
         self.widget.bind("<Enter>", self.on_enter, add="+")
         self.widget.bind("<Leave>", self.on_leave, add="+")
         self.widget.bind("<Motion>", self.on_enter, add="+")
         self.widget.bind("<B1-Motion>", self.on_enter, add="+")
         self.widget.bind("<Destroy>", lambda _: self.hide(), add="+")
-        
+
     def show(self) -> None:
         """
         Enable the widget.
         """
         self.disable = False
-        
+
     def on_enter(self, event) -> None:
         """
         Processes motion within the widget including entering and moving.
         """
 
-        if self.disable: return
+        if self.disable:
+            return
         self.last_moved = time.time()
 
         # Set the status as inside for the very first time
         if self.status == "outside":
             self.status = "inside"
 
         # If the follow flag is not set, motion within the widget will make the ToolTip dissapear
         if not self.follow:
             self.status = "inside"
             self.withdraw()
 
+        # Calculate available space on the right side of the widget relative to the screen
+        root_width = self.winfo_screenwidth()
+        widget_x = event.x_root
+        space_on_right = root_width - widget_x
+
+        # Calculate the width of the tooltip's text based on the length of the message string
+        text_width = self.message_label.winfo_reqwidth()
+
+        # Calculate the offset based on available space and text width to avoid going off-screen on the right side
+        offset_x = self.x_offset
+        if space_on_right < text_width + 20:  # Adjust the threshold as needed
+            offset_x = -text_width - 20  # Negative offset when space is limited on the right side
+
         # Offsets the ToolTip using the coordinates od an event as an origin
-        self.geometry(f"+{event.x_root + self.x_offset}+{event.y_root + self.y_offset}")
+        self.geometry(f"+{event.x_root + offset_x}+{event.y_root + self.y_offset}")
 
         # Time is in integer: milliseconds
         self.after(int(self.delay * 1000), self._show)
 
     def on_leave(self, event=None) -> None:
         """
         Hides the ToolTip temporarily.
@@ -152,42 +170,42 @@
         """
         Displays the ToolTip.
         """
 
         if not self.widget.winfo_exists():
             self.hide()
             self.destroy()
-            
+
         if self.status == "inside" and time.time() - self.last_moved >= self.delay:
             self.status = "visible"
             self.deiconify()
-        
+
     def hide(self) -> None:
         """
         Disable the widget from appearing.
         """
         if not self.winfo_exists():
             return
         self.withdraw()
         self.disable = True
 
     def is_disabled(self) -> None:
         """
         Return the window state
         """
         return self.disable
-    
+
     def get(self) -> None:
         """
         Returns the text on the tooltip.
-        """  
+        """
         return self.messageVar.get()
-    
+
     def configure(self, message: str = None, delay: float = None, bg_color: str = None, **kwargs):
         """
         Set new message or configure the label parameters.
         """
         if delay: self.delay = delay
         if bg_color: self.frame.configure(fg_color=bg_color)
-        
+
         self.messageVar.set(message)
         self.message_label.configure(**kwargs)
```

### Comparing `CTkToolTip-0.7/CTkToolTip.egg-info/PKG-INFO` & `CTkToolTip-0.8/CTkToolTip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkToolTip
-Version: 0.7
+Version: 0.8
 Summary: Customtkinter Tooltip widget
 Home-page: https://github.com/Akascape/CTkToolTip
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,tooltips,popup,widgets,tkinter-widgets,tooltip popup,floating window
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -15,19 +15,20 @@
 
 # CTkToolTip
 **Small tooltip pop-up label for displaying details on customtkinter widgets.**
 
 ![example](https://user-images.githubusercontent.com/89206401/229771216-199727ef-2a01-4ab3-bac6-7e0a5234389e.gif)
 
 ## Features
-- Display over any widget
+- Display over any CTk widget
 - Configurable options
 - Transparency effect
 - Round corners
-- Can show current value of a CTk Slider
+- Can be used with CTkSlider to show the value
+- Dynamic offset
 - Add delays
 
 ## Installation
 
 ```
 pip install CTkToolTip
 ```
@@ -79,15 +80,15 @@
 | corner_radius | roundness of the corners |
 | border_width | add a border around the tooltips (default is 0) |
 | border_color | change the color of the border width |
 | padding | add padx and pady inside the tooltip frame, tuple: (padx, pady) |
 | **text_color** | change the text color of tooltip |
 | wraplength | constrains the width of the tooltip, causing CTkToolTip, where required, to wrap the message at word boundaries. |
 | font | label text font, tuple: (font_name, size) |
-| justify | change the text display structure (left, right or center |
+| justify | change the text display structure (left, right or center) |
 | _*Other Label Parameters_ | _All other parameters for ctk label can be passed in ctktooltip_ |
 
 ## Methods
 
 - **.configure(message, arguments...)**
 
    configure the text and other parameters for the tooltip
```

### Comparing `CTkToolTip-0.7/LICENSE` & `CTkToolTip-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkToolTip-0.7/PKG-INFO` & `CTkToolTip-0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkToolTip
-Version: 0.7
+Version: 0.8
 Summary: Customtkinter Tooltip widget
 Home-page: https://github.com/Akascape/CTkToolTip
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,tooltips,popup,widgets,tkinter-widgets,tooltip popup,floating window
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -15,19 +15,20 @@
 
 # CTkToolTip
 **Small tooltip pop-up label for displaying details on customtkinter widgets.**
 
 ![example](https://user-images.githubusercontent.com/89206401/229771216-199727ef-2a01-4ab3-bac6-7e0a5234389e.gif)
 
 ## Features
-- Display over any widget
+- Display over any CTk widget
 - Configurable options
 - Transparency effect
 - Round corners
-- Can show current value of a CTk Slider
+- Can be used with CTkSlider to show the value
+- Dynamic offset
 - Add delays
 
 ## Installation
 
 ```
 pip install CTkToolTip
 ```
@@ -79,15 +80,15 @@
 | corner_radius | roundness of the corners |
 | border_width | add a border around the tooltips (default is 0) |
 | border_color | change the color of the border width |
 | padding | add padx and pady inside the tooltip frame, tuple: (padx, pady) |
 | **text_color** | change the text color of tooltip |
 | wraplength | constrains the width of the tooltip, causing CTkToolTip, where required, to wrap the message at word boundaries. |
 | font | label text font, tuple: (font_name, size) |
-| justify | change the text display structure (left, right or center |
+| justify | change the text display structure (left, right or center) |
 | _*Other Label Parameters_ | _All other parameters for ctk label can be passed in ctktooltip_ |
 
 ## Methods
 
 - **.configure(message, arguments...)**
 
    configure the text and other parameters for the tooltip
```

### Comparing `CTkToolTip-0.7/README.md` & `CTkToolTip-0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # CTkToolTip
 **Small tooltip pop-up label for displaying details on customtkinter widgets.**
 
 ![example](https://user-images.githubusercontent.com/89206401/229771216-199727ef-2a01-4ab3-bac6-7e0a5234389e.gif)
 
 ## Features
-- Display over any widget
+- Display over any CTk widget
 - Configurable options
 - Transparency effect
 - Round corners
-- Can show current value of a CTk Slider
+- Can be used with CTkSlider to show the value
+- Dynamic offset
 - Add delays
 
 ## Installation
 
 ```
 pip install CTkToolTip
 ```
@@ -64,15 +65,15 @@
 | corner_radius | roundness of the corners |
 | border_width | add a border around the tooltips (default is 0) |
 | border_color | change the color of the border width |
 | padding | add padx and pady inside the tooltip frame, tuple: (padx, pady) |
 | **text_color** | change the text color of tooltip |
 | wraplength | constrains the width of the tooltip, causing CTkToolTip, where required, to wrap the message at word boundaries. |
 | font | label text font, tuple: (font_name, size) |
-| justify | change the text display structure (left, right or center |
+| justify | change the text display structure (left, right or center) |
 | _*Other Label Parameters_ | _All other parameters for ctk label can be passed in ctktooltip_ |
 
 ## Methods
 
 - **.configure(message, arguments...)**
 
    configure the text and other parameters for the tooltip
```

### Comparing `CTkToolTip-0.7/setup.cfg` & `CTkToolTip-0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 546f 6f6c 5469 700d 0a76   = CTkToolTip..v
-00000020: 6572 7369 6f6e 203d 2030 2e37 0d0a 6465  ersion = 0.7..de
+00000020: 6572 7369 6f6e 203d 2030 2e38 0d0a 6465  ersion = 0.8..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4375 7374  scription = Cust
 00000040: 6f6d 746b 696e 7465 7220 546f 6f6c 7469  omtkinter Toolti
 00000050: 700d 0a6c 6f6e 675f 6465 7363 7269 7074  p..long_descript
 00000060: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
 00000070: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 00000080: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
 00000090: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
```

### Comparing `CTkToolTip-0.7/setup.py` & `CTkToolTip-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name='CTkToolTip',
-    version='0.7',
+    version='0.8',
     description="Customtkinter Tooltip widget",
     license="Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type="text/markdown",
     author='Akash Bora',
     url="https://github.com/Akascape/CTkToolTip",
```

