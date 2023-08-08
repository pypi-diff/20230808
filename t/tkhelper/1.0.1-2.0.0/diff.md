# Comparing `tmp/tkhelper-1.0.1.tar.gz` & `tmp/tkhelper-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tkhelper-1.0.1.tar", last modified: Mon Jul 13 06:46:32 2020, max compression
+gzip compressed data, was "tkhelper-2.0.0.tar", last modified: Tue Aug  8 12:56:39 2023, max compression
```

## Comparing `tkhelper-1.0.1.tar` & `tkhelper-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2020-07-13 06:46:32.000000 tkhelper-1.0.1/
--rw-rw-rw-   0        0        0     3107 2020-07-13 06:46:32.000000 tkhelper-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1902 2020-07-12 19:11:23.000000 tkhelper-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2020-07-13 06:46:32.000000 tkhelper-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      755 2020-07-13 06:44:46.000000 tkhelper-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2020-07-13 06:46:32.000000 tkhelper-1.0.1/tkhelper/
--rw-rw-rw-   0        0        0        0 2020-07-12 15:55:13.000000 tkhelper-1.0.1/tkhelper/__init__.py
--rw-rw-rw-   0        0        0       94 2020-07-13 06:43:47.000000 tkhelper-1.0.1/tkhelper/package_info.py
-drwxrwxrwx   0        0        0        0 2020-07-13 06:46:32.000000 tkhelper-1.0.1/tkhelper/progressbars/
--rw-rw-rw-   0        0        0        0 2020-07-13 06:27:21.000000 tkhelper-1.0.1/tkhelper/progressbars/__init__.py
--rw-rw-rw-   0        0        0    32616 2020-07-13 06:44:17.000000 tkhelper-1.0.1/tkhelper/progressbars/circular.py
--rw-rw-rw-   0        0        0    32102 2020-07-13 06:45:24.000000 tkhelper-1.0.1/tkhelper/widgets.py
-drwxrwxrwx   0        0        0        0 2020-07-13 06:46:32.000000 tkhelper-1.0.1/tkhelper.egg-info/
--rw-rw-rw-   0        0        0     3107 2020-07-13 06:46:32.000000 tkhelper-1.0.1/tkhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2020-07-13 06:46:32.000000 tkhelper-1.0.1/tkhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-13 06:46:32.000000 tkhelper-1.0.1/tkhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2020-07-13 06:46:32.000000 tkhelper-1.0.1/tkhelper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 12:56:39.888918 tkhelper-2.0.0/
+-rw-rw-rw-   0        0        0     1071 2020-06-24 20:49:09.000000 tkhelper-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2456 2023-08-08 12:56:39.888918 tkhelper-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1902 2020-07-12 19:11:23.000000 tkhelper-2.0.0/README.md
+-rw-rw-rw-   0        0        0     1280 2023-08-08 12:55:32.000000 tkhelper-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       31 2023-08-06 09:22:40.000000 tkhelper-2.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 12:56:39.889918 tkhelper-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 12:56:39.825874 tkhelper-2.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2020-07-12 18:07:26.000000 tkhelper-2.0.0/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:56:39.845874 tkhelper-2.0.0/tkhelper/
+-rw-rw-rw-   0        0        0        0 2020-07-12 15:55:13.000000 tkhelper-2.0.0/tkhelper/__init__.py
+-rw-rw-rw-   0        0        0      116 2023-08-08 10:05:17.000000 tkhelper-2.0.0/tkhelper/package_info.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:56:39.886918 tkhelper-2.0.0/tkhelper/progressbars/
+-rw-rw-rw-   0        0        0        0 2023-08-04 13:17:26.000000 tkhelper-2.0.0/tkhelper/progressbars/__init__.py
+-rw-rw-rw-   0        0        0    39844 2023-08-08 06:42:14.000000 tkhelper-2.0.0/tkhelper/progressbars/circular.py
+-rw-rw-rw-   0        0        0    48907 2023-08-08 11:10:17.000000 tkhelper-2.0.0/tkhelper/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:56:39.871918 tkhelper-2.0.0/tkhelper.egg-info/
+-rw-rw-rw-   0        0        0     2456 2023-08-08 12:56:39.000000 tkhelper-2.0.0/tkhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-08-08 12:56:39.000000 tkhelper-2.0.0/tkhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 12:56:39.000000 tkhelper-2.0.0/tkhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-08 12:56:39.000000 tkhelper-2.0.0/tkhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 12:56:39.000000 tkhelper-2.0.0/tkhelper.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tkhelper-1.0.1/PKG-INFO` & `tkhelper-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,88 @@
-Metadata-Version: 2.1
-Name: tkhelper
-Version: 1.0.1
-Summary: A module to display some customized tkinter modules
-Home-page: https://github.com/erdoganonal/tk_helper
-Author: Erdogan Onal
-Author-email: erdoganonal@windowslive.com
-License: UNKNOWN
-Description: # Tkinter Helper
-        
-        A module to display some customized tkinter modules.
-        
-        ## Getting Started
-        
-        You may download this project directly from GitHub, or you may use Python's package manager(pip).
-        
-        ### Prerequisites
-        
-        Please see [requirements.txt](requirements.txt) for prerequisites.
-        
-        ### Installing
-        
-        Use pip to install this library.
-        
-        ```cmd, bash
-        pip install tkhelper
-        ```
-        
-        ## Running the tests
-        
-        Doctests and unit tests can be run.
-        
-        ### Running doctests
-        
-        Use python doctest.
-        
-        ```cmd, bash
-        python -m doctest tkhelper\widgets.py tkhelper\progressbars\circular.py
-        ```
-        
-        ### Running unit tests
-        
-        Unit tests still in development.
-        
-        ## Example Usage
-        
-        ```python
-        import tkinter as tk
-        from tkhelper.widgets import ResizableLabel, ResizableButton
-        from tkhelper.progressbars.circular import TransparentSpinnerBar, SpinnerLoadingBar
-        
-        root = tk.Tk()
-        
-        circular_bar = TransparentSpinnerBar(root, kind=SpinnerLoadingBar)
-        def start_bar():
-            circular_bar.start()
-            resizable_button.config(
-                command=stop_bar,
-                text="Click the button to stop the circular loading bar"
-            )
-        
-        def stop_bar():
-            circular_bar.stop()
-            resizable_button.config(
-                command=start_bar,
-                text="Click the button to run the circular loading bar"
-            )
-        
-        
-        resizable_label = ResizableLabel(
-            root, text="Example resizable label",
-            weight=0.9, resize=True
-        )
-        resizable_label.grid()
-        
-        resizable_button = ResizableButton(
-            root, text="Click the button to run the circular loading bar",
-            weight=0.5, resize=True, command=start_bar
-        )
-        resizable_button.grid()
-        
-        root.geometry("500x500")
-        root.mainloop()
-        ```
-        
-        ## Version Info
-        
-        Version 1.0.0.
-        
-        ## Authors
-        
-        * **Erdogan Onal** - *Owner* - [Erdogan Onal](https://github.com/erdoganonal)
-        
-        ## License
-        
-        This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
-Description-Content-Type: text/markdown
+# Tkinter Helper
+
+A module to display some customized tkinter modules.
+
+## Getting Started
+
+You may download this project directly from GitHub, or you may use Python's package manager(pip).
+
+### Prerequisites
+
+Please see [requirements.txt](requirements.txt) for prerequisites.
+
+### Installing
+
+Use pip to install this library.
+
+```cmd, bash
+pip install tkhelper
+```
+
+## Running the tests
+
+Doctests and unit tests can be run.
+
+### Running doctests
+
+Use python doctest.
+
+```cmd, bash
+python -m doctest tkhelper\widgets.py tkhelper\progressbars\circular.py
+```
+
+### Running unit tests
+
+Unit tests still in development.
+
+## Example Usage
+
+```python
+import tkinter as tk
+from tkhelper.widgets import ResizableLabel, ResizableButton
+from tkhelper.progressbars.circular import TransparentSpinnerBar, SpinnerLoadingBar
+
+root = tk.Tk()
+
+circular_bar = TransparentSpinnerBar(root, kind=SpinnerLoadingBar)
+def start_bar():
+    circular_bar.start()
+    resizable_button.config(
+        command=stop_bar,
+        text="Click the button to stop the circular loading bar"
+    )
+
+def stop_bar():
+    circular_bar.stop()
+    resizable_button.config(
+        command=start_bar,
+        text="Click the button to run the circular loading bar"
+    )
+
+
+resizable_label = ResizableLabel(
+    root, text="Example resizable label",
+    weight=0.9, resize=True
+)
+resizable_label.grid()
+
+resizable_button = ResizableButton(
+    root, text="Click the button to run the circular loading bar",
+    weight=0.5, resize=True, command=start_bar
+)
+resizable_button.grid()
+
+root.geometry("500x500")
+root.mainloop()
+```
+
+## Version Info
+
+Version 1.0.0.
+
+## Authors
+
+* **Erdogan Onal** - *Owner* - [Erdogan Onal](https://github.com/erdoganonal)
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `tkhelper-1.0.1/tkhelper/progressbars/circular.py` & `tkhelper-2.0.0/tkhelper/progressbars/circular.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,143 +1,135 @@
 """Renders a widget using tk.Canvas module to
 busy the screen for a while
 """
 import abc
-import math
 import enum
-from typing import Any, Union, Iterable, Tuple, Optional, Generator, Type
-from collections import deque
+import math
 import string
-
 import tkinter as tk
-from colour import Color
-
-from ..package_info import __version__, __author__, __mail__
+from collections import deque
+from dataclasses import dataclass
+from tkinter.font import Font
+from typing import Any, Callable, Deque, Dict, Generator, Iterable, List, Optional, Tuple, Type, TypeAlias, Union
 
+from colour import Color  # type:ignore[import]
 
 FULL_CIRCLE_DEGREE = 360
 
+_ColorType: TypeAlias = Tuple[str, str, str, str, str, str, str, str]
 
 # pylint: disable=too-many-ancestors
+# pylint: disable=too-many-lines
 
 
-def _change_text(root, label: tk.Label, *p_bars, remaining_time: int = 2):
+def _change_text(root: tk.Misc, label: tk.Label, *p_bars: "CircularLoadingBarBase", remaining_time: int = 2) -> None:
     """helper function for docstrings"""
     for p_bar in p_bars:
         if not p_bar.is_active:
             p_bar.start()
-    label.config(
-        text="Bar will be stopped in {0} seconds".format(remaining_time)
-    )
+    label.config(text=f"Bar will be stopped in {remaining_time} seconds")
     if remaining_time <= 0:
         for p_bar in p_bars:
             p_bar.stop()
-        label.config(
-            text="The window will be destroyed in a second"
-        )
+        label.config(text="The window will be destroyed in a second")
         root.after(1000, root.destroy)
     else:
-        root.after(1000, lambda: _change_text(
-            root, label, *p_bars, remaining_time=remaining_time - 1
-        ))
+        root.after(1000, lambda: _change_text(root, label, *p_bars, remaining_time=remaining_time - 1))
 
 
 class InconsistentLengths(Exception):
     """Raise when MaskItem lengths are not match"""
 
     def __init__(self, expected_length: int, actual_length: int):
-        super().__init__(
-            "Expected length of {0}, got {1}"
-            "".format(expected_length, actual_length)
-        )
+        super().__init__(f"Expected length of {expected_length}, got {actual_length}")
 
 
 class _EnumBase(enum.Enum):
     @classmethod
     def raise_bad_value(cls, value: Any, safe: bool = False) -> None:
         """raises ValueError when given value is not valid"""
         if safe:
             try:
                 if value in cls:
                     return
             except TypeError:
                 pass
-        values = [repr(item) for item in cls.__dict__['_member_map_'].values()]
+        values = [repr(item) for item in cls]
 
-        other_value = ''
+        other_value = ""
         if len(values) > 1:
             values, other_value = values[:-1], values[-1]
-            other_value = ' or {0}'.format(other_value)
-        raise ValueError(
-            "bad value \"{0!r}\": expected {1}{2}"
-            "".format(value, ', '.join(values), other_value)
-        )
+            other_value = f" or {other_value}"
+        raise ValueError(f'bad value "{value!r}": expected {", ".join(values)}{other_value}')
 
 
 class ResizeActions(_EnumBase):
     """Actions for resize"""
 
-    ADD = 'add'
-    SET = 'set'
-    SUB = 'subtract'
+    ADD = "add"
+    SET = "set"
+    SUB = "subtract"
 
 
 class AngleType(_EnumBase):
     """Angle types"""
 
-    DEGREE = 'degree'
-    RADIAN = 'radian'
+    DEGREE = "degree"
+    RADIAN = "radian"
+
+
+# pylint: disable=too-few-public-methods
+class Colors:
+    """Holds pre-defined 8 length color range"""
+
+    GRAYED = ("#fafafa", "#f5f5f5", "#e0e0e0", "#bdbdbd", "#9e9e9e", "#757575", "#616161", "#424242")
+    RAINBOW = ("#fff100", "#ff8c00", "#e81123", "#4b0082", "#000080", "#00188f", "#00b294", "#bad80a")
+    BLACK = ("black", "black", "black", "black", "black", "black", "black", "black")
 
 
 class Converter:
     """Math calculations between circles"""
 
     @staticmethod
-    def centered_circle_to_circle(center_x, center_y, radius):
+    def centered_circle_to_circle(center_x: int, center_y: int, radius: float) -> Tuple[int, int, float]:
         """Converts centered_circle to circle"""
-        return center_x - radius, center_y - radius, radius
+        return int(center_x - radius), int(center_y - radius), radius
 
     @classmethod
-    def centered_circle_to_oval(cls, center_x, center_y, radius):
+    def centered_circle_to_oval(cls, center_x: int, center_y: int, radius: float) -> Tuple[int, int, int, int]:
         """Converts centered circle to oval"""
-        return cls.circle_to_oval(
-            *cls.centered_circle_to_circle(center_x, center_y, radius)
-        )
+        return cls.circle_to_oval(*cls.centered_circle_to_circle(center_x, center_y, radius))
 
     @staticmethod
-    def circle_to_oval(start_x, start_y, radius):
+    def circle_to_oval(start_x: int, start_y: int, radius: float) -> Tuple[int, int, int, int]:
         """Converts circle to oval"""
-        diameter = 2 * radius
+        diameter = int(2 * radius)
         end_x = start_x + diameter
         end_y = start_y + diameter
         return start_x, start_y, end_x, end_y
 
     @staticmethod
-    def oval_to_circle(start_x, start_y, end_x, end_y):
+    def oval_to_circle(start_x: int, start_y: int, end_x: int, end_y: int) -> Tuple[int, int, float]:
         """Converts oval to circle"""
         assert end_x == end_y, "Oval must be circle"
         return start_x, start_y, (end_x - start_x) / 2
 
     @staticmethod
-    def circle_to_centered_circle(start_x, start_y, radius):
+    def circle_to_centered_circle(start_x: int, start_y: int, radius: float) -> Tuple[int, int, float]:
         """Converts circle to centered circle"""
-        return start_x + radius, start_y + radius, radius
+        return int(start_x + radius), int(start_y + radius), radius
 
     @classmethod
-    def oval_to_centered_circle(cls, start_x, start_y, end_x, end_y):
+    def oval_to_centered_circle(cls, start_x: int, start_y: int, end_x: int, end_y: int) -> Tuple[int, int, float]:
         """Converts oval to centered circle"""
-        return cls.circle_to_centered_circle(
-            *cls.oval_to_circle(start_x, start_y, end_x, end_y)
-        )
+        return cls.circle_to_centered_circle(*cls.oval_to_circle(start_x, start_y, end_x, end_y))
 
 
 _MaskItemTest = type("_MaskItemTest", (), {})
-_MaskItemTest.test_method = staticmethod(
-    lambda test_param: print(test_param.copy())
-)
+_MaskItemTest.test_method = staticmethod(lambda test_param: print(test_param.copy()))  # type: ignore[attr-defined]
 
 
 class MaskItem:
     """An item for the mask. This is actually a mask to apply
     on the items for every loop.
         Args:
             method_name: The function name of the target class
@@ -149,17 +141,17 @@
         ...     method_name='test_method', test_param=range(10)
         ... )
         >>> method = getattr(_MaskItemTest(), mask.name)
         >>> method(**getattr(mask, '_kwargs'))
         deque([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     """
 
-    def __init__(self, method_name: str, **kwargs: Iterable):
+    def __init__(self, method_name: str, **kwargs: Any):
         self._method_name = method_name
-        self._kwargs = {}
+        self._kwargs: Dict[str, Deque[Any]] = {}
 
         length = None
         for key, value in kwargs.items():
             value = deque(value)
             if length is None:
                 length = len(value)
             elif length != len(value):
@@ -169,72 +161,84 @@
     @property
     def name(self) -> str:
         """Returns the method name which will be called from given object"""
         return self._method_name
 
     def rotate(self, rotate_by: int = 1) -> None:
         """Shift entire mask items by one"""
-        for key in self._kwargs:
-            self._kwargs[key].rotate(rotate_by)
+        for value in self._kwargs.values():
+            value.rotate(rotate_by)
 
     def __len__(self) -> int:
         for value in self._kwargs.values():
             return len(value)
         return 0
 
-    def __iter__(self) -> Tuple[str, Any]:
+    def __iter__(self) -> Generator[Tuple[str, Any], None, None]:
         for key, value in self._kwargs.items():
             yield key, value
 
     def __str__(self) -> str:
-        string_result = "Method name: {0}\n".format(self.name)
+        string_result = f"Method name: {self.name}\n"
         for param, value in self._kwargs.items():
-            string_result += "\t{0}: {1}\n".format(param, value)
+            string_result += f"\t{param}: {value}\n"
         return string_result
 
 
-class Mask(list):
+class Mask(list[MaskItem]):
     """
     A list that includes masks.
         Args:
             *args: List of MaskItems
     """
 
     def __init__(self, *args: MaskItem, rotate_by: int = 1):
         super().__init__(args)
         self.rotate_by = rotate_by
 
-    def apply(self, obj: Any) -> None:
+    def apply(self, obj: "CircularLoadingBarBase") -> None:
         """Apply the mask on given items"""
         for idx, item_id in enumerate(obj.items):
             for mask_item in self:
                 method = getattr(obj, mask_item.name)
                 for param, value in mask_item:
                     method(item_id, **{param: value[idx]})
 
         self.rotate(self.rotate_by)
 
     def rotate(self, rotate_by: int = 1) -> None:
         """Shift the mask by one"""
         for mask_item in self:
             mask_item.rotate(rotate_by)
 
-    def __len__(self) -> None:
+    def __len__(self) -> int:
         length = None
         for mask_item in self:
             if length is None:
                 length = len(mask_item)
             elif length != len(mask_item):
                 raise InconsistentLengths(length, len(mask_item))
         return length or 0
 
     def __str__(self) -> str:
         return "\n".join(str(i) for i in self)
 
 
+@dataclass(frozen=True)
+class ProgressOptions:
+    """Options for progress"""
+
+    stop_bar_when_max: bool = False
+    stop_callback: Optional[Callable[[], Any]] = None
+    destroy_when_max: bool = False
+    destroy_callback: Optional[Callable[[], Any]] = None
+    color: str = "black"
+    font: Union[str, Font] = "Helvetica 15 bold"
+
+
 class CircularLoadingBarBase(tk.Canvas, metaclass=abc.ABCMeta):
     """Base for loading bar
 
         Args:
             *args
             **kwargs: Parameters for tk.Canvas module
             size:     If passed, the width and height of canvas will be
@@ -245,44 +249,52 @@
         Traceback (most recent call last):
             ...
         TypeError: Can't instantiate abstract class \
 CircularLoadingBarBase with abstract methods items, update_bar
     """
 
     def __init__(
-            self, *args, mask: Mask,
-            size: Optional[int] = None,
-            shift: int = 0, **kwargs):
-        if size is not None:
-            kwargs['width'] = kwargs['height'] = size
-        super().__init__(*args, **kwargs)
+        self,
+        *canvas_args: Any,
+        mask: Mask,
+        size: Optional[int] = None,
+        shift: int = 0,
+        progress_options: Optional[ProgressOptions] = None,
+        **canvas_kwargs: Any,
+    ) -> None:
+        if size is None:
+            size = 250
+
+        canvas_kwargs["width"] = canvas_kwargs["height"] = size
+
+        super().__init__(*canvas_args, **canvas_kwargs)
 
         self.shift = shift
-        self._is_active = None
+        self._is_active = False
+        self._text_id: Optional[int] = None
+        self._progress = 0.0
+        self._progress_options = progress_options
         self.mask = mask
 
     @property
     def mask(self) -> Mask:
         """Return the mask"""
         return self._mask
 
     @mask.setter
     def mask(self, mask: Mask) -> None:
         """Set the mask"""
         if isinstance(mask, Mask):
             self._mask = mask
         else:
-            raise ValueError(
-                "mask should be instance of"
-                "{0!r}".format(Mask)
-            )
+            raise ValueError(f"mask should be instance of {Mask!r}")
 
     @property
     @abc.abstractmethod
-    def items(self):
+    def items(self) -> List[int]:
         """Returns the items that the mask will be applied to."""
 
     @staticmethod
     def get_sequence(start: float, stop: float, count: float) -> Generator[float, None, None]:
         """Returns a generator that yields points between start and stop.
         The start point is included and the stop point is not. [start, stop)
         Step will be calculated based on count.
@@ -315,21 +327,19 @@
         with that kind of operations
         >>> math.cos(math.pi/2)
         6.123233995736766e-17
 
         >>> CircularLoadingBarBase.to_float(math.cos(math.pi/2))
         0.0
         """
-        precision = 10 ** precision
+        precision = 10**precision
         return int(num * precision) / precision
 
     @classmethod
-    def polar_to_cartesian(
-            cls, radius: float, angle: float,
-            kind: AngleType = AngleType.DEGREE) -> Tuple[float, float]:
+    def polar_to_cartesian(cls, radius: float, angle: float, kind: AngleType = AngleType.DEGREE) -> Tuple[float, float]:
         """Calculates the cartesian coordinates from polar coordinates.
         Args:
             radius: The radius of the polar coordinates
             angle:  The angle of the polar coordinates
             kind:   Could be degree or radian.
         Formula:
             x = radius + radius * sin(alpha)
@@ -365,84 +375,113 @@
 
     @property
     def is_active(self) -> bool:
         """return True if bar is active, False otherwise"""
         return self._is_active
 
     @property
-    def size(self) -> int:
+    def fit_size(self) -> int:
         """return the size to fit the widget"""
         return min(self.winfo_width(), self.winfo_height())
 
     @abc.abstractmethod
     def update_bar(self) -> None:
         """updates the loading bar attributes"""
 
+    def _add_progress_text(self) -> None:
+        if self._text_id is not None:
+            raise RuntimeError("Progress text already created")
+
+        if self._progress_options is None:
+            return
+
+        self._text_id = self.create_text(
+            int(self.cget("width")) / 2,
+            int(self.cget("width")) / 2,
+            text="00.00",
+            fill=self._progress_options.color,
+            font=self._progress_options.font,
+            anchor=tk.CENTER,
+        )
+
+    def update_progress(self, update_by: float = 1.0) -> float:
+        """updates the loading progress"""
+        if self._progress_options is None or self._text_id is None:
+            return -1
+
+        self._progress += update_by
+        if self._progress > 100:
+            if self._progress_options.stop_bar_when_max:
+                self.stop()
+                if self._progress_options.stop_callback:
+                    self._progress_options.stop_callback()
+            if self._progress_options.destroy_when_max:
+                self.destroy()
+                if self._progress_options.destroy_callback:
+                    self._progress_options.destroy_callback()
+        else:
+            self.itemconfigure(self._text_id, text=f"{self._progress:.2f}")
+
+        return self._progress
+
     def _start(self, interval_ms: int) -> None:
         if not self.is_active:
             return
 
         self.update_bar()
         self.mask.apply(self)
         self.after(interval_ms, self._start, interval_ms)
 
     def start(self, interval_ms: int = 100) -> None:
         """starts the circle loading bar"""
         if self.is_active:
             return
 
+        if self._progress_options is not None:
+            self._add_progress_text()
+
         self._is_active = True
         self._start(interval_ms=interval_ms)
 
     def stop(self) -> None:
         """stop the bar"""
+        self._progress = 0.0
+        self._text_id = None
         self._is_active = False
 
-    def create_centered_circle(
-            self, center_x: float, center_y: float,
-            radius: float, **kwargs) -> int:
+    def create_centered_circle(self, center_x: int, center_y: int, radius: float, **kwargs: Any) -> int:
         """Create a circle with given radius and coordinates
-            that pointing the center of the circle
+        that pointing the center of the circle
 
-            Args:
-                center_x: x coordinate of the circle in cartesian system
-                center_y: y coordinate of the circle in cartesian system
-                radius:   Radius of the circle
-            Returns:
-                id of the created circle
+        Args:
+            center_x: x coordinate of the circle in cartesian system
+            center_y: y coordinate of the circle in cartesian system
+            radius:   Radius of the circle
+        Returns:
+            id of the created circle
         """
-        return self.create_oval(
-            Converter.centered_circle_to_oval(
-                center_x, center_y, radius
-            ), **kwargs
-        )
+        return self.create_oval(Converter.centered_circle_to_oval(center_x, center_y, radius), **kwargs)
 
-    def create_circle(self, start_x: float, start_y: float, radius: float, **kwargs) -> int:
+    def create_circle(self, start_x: int, start_y: int, radius: float, **kwargs: Any) -> int:
         """Create a circle with given radius and place to given coordinates
-            Args:
-                start_x: x origin point of the square which includes the circle
-                start_y: y origin point of the square which includes the circle
-                radius:  Radius of the circle
-            Returns:
-                id of the created circle
+        Args:
+            start_x: x origin point of the square which includes the circle
+            start_y: y origin point of the square which includes the circle
+            radius:  Radius of the circle
+        Returns:
+            id of the created circle
         """
-        return self.create_oval(
-            Converter.circle_to_oval(
-                start_x, start_y, radius
-            ), **kwargs
-        )
+        return self.create_oval(Converter.circle_to_oval(start_x, start_y, radius), **kwargs)
 
-    def resize(
-            self, item_id: int, radius: float,
-            action: ResizeActions = ResizeActions.SET) -> None:
+    def resize(self, item_id: int, radius: float, action: ResizeActions = ResizeActions.SET) -> None:
         """Resize given circle. New radius will be applied based on the action
-            Args:
-                item_id: Id of the circle
-                radius:  New value to apply on the radius
-                action:  The action to apply on the old radius
+        Args:
+            item_id: Id of the circle
+            radius:  New value to apply on the radius
+            action:  The action to apply on the old radius
         """
         start_x, start_y, end_x, end_y = self.coords(item_id)
 
         old_radius = self.to_float((end_x - start_x) / 2, 1)
 
         if action == ResizeActions.SET:
             # set new radius
@@ -455,97 +494,103 @@
             ResizeActions.raise_bad_value(action)
 
         end_x = start_x + 2 * radius
         end_y = start_y + 2 * radius
 
         self.coords(item_id, start_x, start_y, end_x, end_y)
 
-    def __del__(self):
+    def __del__(self) -> None:
         try:
             self.stop()
+            self.update()
         except AttributeError:
             pass
 
 
 class SpinningCirclesLoadingBarBase(CircularLoadingBarBase):
     """Creates an circular loading bar which consisting circles
 
-        Args:
-            *args
-            **kwargs: Parameters for SpinningCirclesLoadingBarBase module
-            mask:     The list will be applied and rotated every loop.
-            offset:   The offset value to avoid inner circle overflow.
+    Args:
+        *args
+        **kwargs: Parameters for SpinningCirclesLoadingBarBase module
+        mask:     The list will be applied and rotated every loop.
+        offset:   The offset value to avoid inner circle overflow.
     """
 
-    def __init__(self, *args, offset: Optional[Iterable] = None, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self,
+        *canvas_args: Any,
+        offset: Optional[int] = None,
+        mask: Mask,
+        size: Optional[int] = None,
+        shift: int = 0,
+        progress_options: Optional[ProgressOptions] = None,
+        **canvas_kwargs: Any,
+    ) -> None:
+        super().__init__(*canvas_args, mask=mask, size=size, shift=shift, progress_options=progress_options, **canvas_kwargs)
 
-        self.circles = []
+        self.circles: List[int] = []
         self.offset = offset
 
     @property
-    def items(self):
+    def items(self) -> List[int]:
         return self.circles
 
     def update_bar(self) -> None:
-        width = self.size / 2
+        width = self.fit_size / 2
         radius = width / 8
         offset = self.offset or 20
 
         for item_id in self.circles:
             self.delete(item_id)
         self.circles = []
 
         for angle in self.get_sequence(0, FULL_CIRCLE_DEGREE, len(self.mask)):
-            coordinate_x, coordinate_y = self.polar_to_cartesian(
-                width - radius - offset, angle)
-            self.circles.append(self.create_centered_circle(
-                coordinate_x + self.shift + radius + offset, coordinate_y +
-                self.shift + radius + offset, radius
-            ))
+            coordinate_x, coordinate_y = self.polar_to_cartesian(width - radius - offset, angle)
+            self.circles.append(
+                self.create_centered_circle(
+                    int(coordinate_x + self.shift + radius + offset),
+                    int(coordinate_y + self.shift + radius + offset),
+                    radius,
+                )
+            )
 
 
 class SpinnerLoadingBar(SpinningCirclesLoadingBarBase):
     """Renders a widget using tk.Canvas module to
     busy the screen for a while. This will give you
     a circle loading bar.
 
     Usage:
         >>> root = tk.Tk()
         >>> root.title("SpinnerLoadingBar")
         ''
         >>> label = tk.Label()
         >>> label.grid()
-        >>> bar1 = SpinnerLoadingBar(root, size=200, colors=SpinnerLoadingBar.GRAYED)
+        >>> bar1 = SpinnerLoadingBar(root, size=200, colors=Colors.GRAYED)
         >>> bar1.grid()
         >>> bar2 = SpinnerLoadingBar(root, size=200)
         >>> bar2.grid()
         >>> _change_text(root, label, bar1, bar2)
 
         >>> root.mainloop()
     """
 
-    GRAYED = (
-        "#fafafa", "#f5f5f5", "#e0e0e0", "#bdbdbd",
-        "#9e9e9e", "#757575", "#616161", "#424242"
-    )
-    RAINBOW = (
-        "#fff100", "#ff8c00", "#e81123", "#4b0082",
-        "#000080", "#00188f", "#00b294", "#bad80a"
-    )
-
-    def __init__(self, *args, colors=None, **kwargs):
-        if colors is None:
-            colors = self.RAINBOW
-
-        kwargs['mask'] = kwargs.get('mask', Mask(
-            MaskItem('itemconfig', fill=colors)
-        ))
-
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self,
+        *canvas_args: Any,
+        colors: _ColorType = Colors.RAINBOW,
+        size: Optional[int] = None,
+        mask: Optional[Mask] = None,
+        shift: int = 0,
+        progress_options: Optional[ProgressOptions] = None,
+        **canvas_kwargs: Any,
+    ) -> None:
+        mask = mask or Mask(MaskItem("itemconfig", fill=colors))
+        super().__init__(*canvas_args, size=size, shift=shift, mask=mask, progress_options=progress_options, **canvas_kwargs)
 
 
 class SpinnerSizedLoadingBar(SpinningCirclesLoadingBarBase):
     """Renders a widget using tk.Canvas module to
     busy the screen for a while. This will give you
     a circular loading bar.
 
@@ -558,250 +603,263 @@
         >>> bar = SpinnerSizedLoadingBar(root, size=200)
         >>> bar.grid()
 
         >>> _change_text(root, label, bar)
         >>> root.mainloop()
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(
+        self,
+        *canvas_args: Any,
+        size: Optional[int] = None,
+        mask: Optional[Mask] = None,
+        shift: int = 0,
+        colors: _ColorType = Colors.BLACK,
+        progress_options: Optional[ProgressOptions] = None,
+        **canvas_kwargs: Any,
+    ) -> None:
         min_radius = 5
         circles = 8
         resize_mask = range(min_radius, min_radius + circles)
         default_mask = Mask(
-            MaskItem('resize', radius=resize_mask),
-            MaskItem('itemconfig', fill=['black'] * len(resize_mask))
+            MaskItem("resize", radius=resize_mask),
+            MaskItem("itemconfig", fill=colors),
         )
 
-        kwargs['mask'] = kwargs.get('mask', default_mask)
-        super().__init__(*args, **kwargs)
+        mask = mask or default_mask
+        super().__init__(*canvas_args, size=size, mask=mask, shift=shift, progress_options=progress_options, **canvas_kwargs)
 
 
 class CircleLoadingBar(CircularLoadingBarBase):
     """Creates a loading bar with color range
 
-        >>> root = tk.Tk()
-        >>> root.title("CircleLoadingBar")
-        ''
-        >>> label = tk.Label()
-        >>> label.grid()
-        >>> bar = CircleLoadingBar(
-        ...     root, size=200, symmetric=True,
-        ...     color1='blue', color2='red'
-        ... )
-        >>> bar.grid()
-        >>> bar.start(interval_ms=8)
-        >>> _change_text(root, label, bar)
-        >>> root.mainloop()
+    >>> root = tk.Tk()
+    >>> root.title("CircleLoadingBar")
+    ''
+    >>> label = tk.Label()
+    >>> label.grid()
+    >>> bar = CircleLoadingBar(
+    ...     root, size=200, symmetric=True,
+    ...     color1='blue', color2='red'
+    ... )
+    >>> bar.grid()
+    >>> bar.start(interval_ms=8)
+    >>> _change_text(root, label, bar)
+    >>> root.mainloop()
     """
+
     DTF_COLOR1 = "#0091c7"
     DTF_COLOR2 = "red"
 
     def __init__(
-            self, *args, width: int = 10,
-            color1: Optional[str] = None, color2: Optional[str] = None,
-            steps: int = 180, color_range: Optional[Iterable] = None,
-            symmetric=True, **kwargs):
+        self,
+        *canvas_args: Any,
+        width: int = 10,
+        color1: Optional[str] = None,
+        color2: Optional[str] = None,
+        steps: int = 180,
+        color_range: Optional[Iterable[str]] = None,
+        symmetric: bool = True,
+        size: Optional[int] = None,
+        shift: int = 0,
+        progress_options: Optional[ProgressOptions] = None,
+        **canvas_kwargs: Any,
+    ) -> None:
         if color_range and (color1 or color2):
-            raise ValueError(
-                "You are not allowed to pass color_range "
-                "and colors at the same time"
-            )
+            raise ValueError("You are not allowed to pass color_range and colors at the same time")
 
         if color1 is None:
             color1 = self.DTF_COLOR1
 
         if color2 is None:
             color2 = self.DTF_COLOR2
 
-        self.arcs = []
+        self.arcs: List[int] = []
         if color_range is None:
             if symmetric:
                 colors = list(self.get_range(color1, color2, int(steps / 2)))
                 color_range = colors + colors[-2::-1]
             else:
                 color_range = self.get_range(color1, color2, steps)
-        kwargs['mask'] = Mask(
-            MaskItem('itemconfig', outline=color_range,),
-            rotate_by=-1
-        )
+        mask = Mask(MaskItem("itemconfig", outline=color_range), rotate_by=-1)
 
         self.width = width
-        self.oval1_id = None
-        self.oval2_id = None
+        self.oval1_id = 0
+        self.oval2_id = 0
 
-        super().__init__(*args, **kwargs)
+        super().__init__(*canvas_args, size=size, mask=mask, shift=shift, progress_options=progress_options, **canvas_kwargs)
 
     @property
-    def items(self):
+    def items(self) -> List[int]:
         return self.arcs
 
-    def update_bar(self):
+    def update_bar(self) -> None:
         outer_circle_offset = self.width
         inner_circle_offset = self.width * 2
         if self.oval1_id:
             self.delete(self.oval1_id)
         if self.oval2_id:
             self.delete(self.oval2_id)
 
         self.oval1_id = self.create_oval(
             outer_circle_offset - self.width / 2,
             outer_circle_offset - self.width / 2,
-            self.size - outer_circle_offset + self.width / 2,
-            self.size - outer_circle_offset + self.width / 2
+            self.fit_size - outer_circle_offset + self.width / 2,
+            self.fit_size - outer_circle_offset + self.width / 2,
         )
 
         self.oval2_id = self.create_oval(
-            inner_circle_offset - self.width / 2, inner_circle_offset - self.width / 2,
-            self.size - inner_circle_offset + self.width /
-            2, self.size - inner_circle_offset + self.width / 2,
+            inner_circle_offset - self.width / 2,
+            inner_circle_offset - self.width / 2,
+            self.fit_size - inner_circle_offset + self.width / 2,
+            self.fit_size - inner_circle_offset + self.width / 2,
         )
 
         self._create_loading_arc(
-            outer_circle_offset, outer_circle_offset,
-            self.size - outer_circle_offset, self.size - outer_circle_offset,
-            width=self.width
+            outer_circle_offset,
+            outer_circle_offset,
+            self.fit_size - outer_circle_offset,
+            self.fit_size - outer_circle_offset,
+            width=self.width,
         )
 
     @staticmethod
-    def get_range(color1: str, color2: str, steps: int) -> Generator:
+    def get_range(color1: str, color2: str, steps: int) -> Generator[str, None, None]:
         """range of color"""
         for color in Color(color1).range_to(color2, steps):
             yield color.get_hex()
 
-    def _create_loading_arc(self, *bbox, width: float, **kwargs) -> None:
+    def _create_loading_arc(self, *bbox: int, width: float, **kwargs: Any) -> None:
         color_range = len(self._mask)
 
-        start = 0
+        start = 0.0
         extent = FULL_CIRCLE_DEGREE / color_range
 
         for arc_id in self.arcs:
             self.delete(arc_id)
 
         self.arcs = []
         for _ in range(len(self.mask)):
             self.arcs.append(
                 self.create_arc(
                     *bbox,
-                    start=start, width=width,
-                    extent=extent, style='arc',
-                    **kwargs
+                    start=start,
+                    width=width,
+                    extent=extent,
+                    style="arc",
+                    **kwargs,
                 )
             )
             start += extent
 
 
 class TransparentSpinnerBar:
     """
-        Places a transparent loading bar
-
-        Args:
-            root[tk.Widget]: A widget to place the loading bar top of it
-            kind[CircularLoadingBarBase]: Type of the loading bar. Should be
-                                        instance of CircularLoadingBarBase.
-            location[
-                Location        : The Location enumeration. Places the loading bar given place.
-                Tuple[int, int] : x and y coordinates. Places the loading bar given place.
-            ]: Optional. Location of the loading bar. Could be Location or Tuple.
-            kwargs: Keyword arguments for the loading bar.
+    Places a transparent loading bar
 
-        >>> root = tk.Tk()
-        >>> root.title("TransparentSpinnerBar")
-        ''
-        >>> label = tk.Label()
-        >>> label.grid()
-        >>> text = tk.Text(root)
-        >>> text.insert("1.0", string.ascii_letters * 50)
-        >>> text.grid()
-        >>> bar = TransparentSpinnerBar(text, kind=SpinnerSizedLoadingBar)
-        >>> _change_text(root, label, bar)
-        >>> root.mainloop()
+    Args:
+        root[tk.Widget]: A widget to place the loading bar top of it
+        kind[CircularLoadingBarBase]: Type of the loading bar. Should be
+                                    instance of CircularLoadingBarBase.
+        location[
+            Location        : The Location enumeration. Places the loading bar given place.
+            Tuple[int, int] : x and y coordinates. Places the loading bar given place.
+        ]: Optional. Location of the loading bar. Could be Location or Tuple.
+        kwargs: Keyword arguments for the loading bar.
+
+    >>> root = tk.Tk()
+    >>> root.title("TransparentSpinnerBar")
+    ''
+    >>> label = tk.Label()
+    >>> label.grid()
+    >>> text = tk.Text(root)
+    >>> text.insert("1.0", string.ascii_letters * 50)
+    >>> text.grid()
+    >>> bar = TransparentSpinnerBar(text, kind=SpinnerSizedLoadingBar)
+    >>> _change_text(root, label, bar)
+    >>> root.mainloop()
     """
 
-    _TRANSPARENT_COLOR = 'white'
+    _TRANSPARENT_COLOR = "white"
 
     class Location(_EnumBase):
         """An enum for positioning the transparent loading bar"""
 
-        LEFT_TOP = 'lt'
-        LEFT_CENTER = 'lc'
-        LEFT_BOTTOM = 'lb'
-
-        MIDDLE_TOP = 'mt'
-        MIDDLE_CENTER = 'mc'
-        MIDDLE_BOTTOM = 'mb'
-
-        RIGHT_TOP = 'rt'
-        RIGHT_CENTER = 'rc'
-        RIGHT_BOTTOM = 'rb'
+        LEFT_TOP = "lt"
+        LEFT_CENTER = "lc"
+        LEFT_BOTTOM = "lb"
+
+        MIDDLE_TOP = "mt"
+        MIDDLE_CENTER = "mc"
+        MIDDLE_BOTTOM = "mb"
+
+        RIGHT_TOP = "rt"
+        RIGHT_CENTER = "rc"
+        RIGHT_BOTTOM = "rb"
 
         @classmethod
-        def is_top(cls, value: Any):
+        def is_top(cls, value: Any) -> bool:
             """Returns True if given value places at the top, False otherwise"""
             return value in (cls.LEFT_TOP, cls.MIDDLE_TOP, cls.RIGHT_TOP)
 
         @classmethod
-        def is_middle(cls, value: Any):
+        def is_middle(cls, value: Any) -> bool:
             """Returns True if given value places at the middle, False otherwise"""
             return value in (cls.MIDDLE_TOP, cls.MIDDLE_CENTER, cls.MIDDLE_BOTTOM)
 
         @classmethod
-        def is_bottom(cls, value: Any):
+        def is_bottom(cls, value: Any) -> bool:
             """Returns True if given value places at the bottom, False otherwise"""
             return value in (cls.LEFT_BOTTOM, cls.MIDDLE_BOTTOM, cls.RIGHT_BOTTOM)
 
         @classmethod
-        def is_left(cls, value: Any):
+        def is_left(cls, value: Any) -> bool:
             """Returns True if given value places at the left, False otherwise"""
             return value in (cls.LEFT_TOP, cls.LEFT_CENTER, cls.LEFT_BOTTOM)
 
         @classmethod
-        def is_center(cls, value: Any):
+        def is_center(cls, value: Any) -> bool:
             """Returns True if given value places at the center, False otherwise"""
             return value in (cls.LEFT_CENTER, cls.MIDDLE_CENTER, cls.RIGHT_CENTER)
 
         @classmethod
-        def is_right(cls, value: Any):
+        def is_right(cls, value: Any) -> bool:
             """Returns True if given value places at the right, False otherwise"""
             return value in (cls.RIGHT_TOP, cls.RIGHT_CENTER, cls.RIGHT_BOTTOM)
 
     def __init__(
-            self, root: Union[tk.Widget, tk.Tk], kind: Type[CircularLoadingBarBase],
-            location: Optional[Union[Location, Tuple[int, int]]] = Location.MIDDLE_CENTER,
-            **kwargs):
+        self,
+        root: Union[tk.Widget, tk.Tk],
+        kind: Type[CircularLoadingBarBase],
+        location: Optional[Union[Location, Tuple[int, int]]] = Location.MIDDLE_CENTER,
+        **kwargs: Any,
+    ) -> None:
         self._root = root
         self.location = location
-        self._main_window = self._loading_bar = None
+        self._main_window: Optional[tk.Toplevel] = None
+        self._loading_bar: Optional[CircularLoadingBarBase] = None
         self.kind = kind
 
         # Override background color
-        kwargs['background'] = kwargs['bg'] = \
-            kwargs['highlightbackground'] = self._TRANSPARENT_COLOR
+        kwargs["background"] = kwargs["bg"] = kwargs["highlightbackground"] = self._TRANSPARENT_COLOR
         self.kwargs = kwargs
 
-        self._root.winfo_toplevel().protocol(
-            "WM_DELETE_WINDOW",
-            self._handle_destroy
-        )
+        self._root.winfo_toplevel().protocol("WM_DELETE_WINDOW", self._handle_destroy)
 
     def _init(self) -> None:
         if self.is_active:
             raise RuntimeError("The bar is already running")
 
         self._main_window = tk.Toplevel(self._root.winfo_toplevel())
-        self._loading_bar = self.kind(
-            self._main_window, **self.kwargs
-        )
+        self._loading_bar = self.kind(self._main_window, **self.kwargs)
         self._loading_bar.grid()
 
-        # TODO: Check for platform dependency
+        # TODO: Check for platform dependency  # pylint: disable=fixme # It is not going to fix in a short term.
         self._main_window.overrideredirect(True)  # Remove the title and border
-        self._main_window.wm_attributes(
-            "-transparentcolor",
-            self._TRANSPARENT_COLOR
-        )
+        self._main_window.wm_attributes("-transparentcolor", self._TRANSPARENT_COLOR)
 
     def _get_coordinates(self) -> Tuple[int, int]:
         """Please refer following schema for positioning"""
         # =============================================================== #
         # *        |      LEFT      #       MIDDLE      #      RIGHT      #
         # =============================================================== #
         #          |      left_x    #      middle_x     #      right_x    #
@@ -817,172 +875,265 @@
         #          |      bottom_y  #      bottom_y     #      bottom_y   #
         # =============================================================== #
 
         try:
             self.Location.raise_bad_value(self.location, safe=True)
         except ValueError:
             # if exact location passed, no need to calculate
-            return self.location
+            return self.location  # type: ignore[return-value]
+
+        if self._loading_bar is None:
+            raise RuntimeError("Cannot get coordinates of uninitialized window")
 
         left_x = self._root.winfo_rootx()
-        middle_x = int(self._root.winfo_rootx() +
-                       self._root.winfo_width() / 2 - self._loading_bar.size / 2)
-        right_x = int(self._root.winfo_rootx() +
-                      self._root.winfo_width() - self._loading_bar.size)
+        middle_x = int(self._root.winfo_rootx() + self._root.winfo_width() / 2 - self._loading_bar.fit_size / 2)
+        right_x = int(self._root.winfo_rootx() + self._root.winfo_width() - self._loading_bar.fit_size)
 
         top_y = self._root.winfo_rooty()
-        center_y = int(self._root.winfo_rooty() +
-                       self._root.winfo_height() / 2 - self._loading_bar.size / 2)
-        bottom_y = int(self._root.winfo_rooty() +
-                       self._root.winfo_height() - self._loading_bar.size)
+        center_y = int(self._root.winfo_rooty() + self._root.winfo_height() / 2 - self._loading_bar.fit_size / 2)
+        bottom_y = int(self._root.winfo_rooty() + self._root.winfo_height() - self._loading_bar.fit_size)
 
-        x_coord = y_coord = None
+        x_coord = y_coord = 0
 
         if self.Location.is_left(self.location):
             x_coord = left_x
-        if self.Location.is_middle(self.location):
+        elif self.Location.is_middle(self.location):
             x_coord = middle_x
-        if self.Location.is_right(self.location):
+        elif self.Location.is_right(self.location):
             x_coord = right_x
 
         if self.Location.is_top(self.location):
             y_coord = top_y
-        if self.Location.is_center(self.location):
+        elif self.Location.is_center(self.location):
             y_coord = center_y
-        if self.Location.is_bottom(self.location):
+        elif self.Location.is_bottom(self.location):
             y_coord = bottom_y
 
         return x_coord, y_coord
 
     def _locate(self) -> None:
         try:
             coord_x, coord_y = self._get_coordinates()
         except tk.TclError:
             return
 
-        self._main_window.geometry('+{}+{}'.format(
-            coord_x, coord_y
-        ))
+        if self._main_window is None:
+            raise RuntimeError("Cannot locate uninitialized window")
+
+        self._main_window.geometry(f"+{coord_x}+{coord_y}")
         if self.is_active:
             self._main_window.after(1, self._locate)
 
-    def _to_top(self):
+    def _to_top(self) -> None:
+        if self._main_window is None:
+            raise RuntimeError("Cannot top uninitialized window")
+
         self._main_window.update_idletasks()
         # put the root window behind the bar
         self._main_window.lift(self._root.winfo_toplevel())
         self._main_window.after(100, self._to_top)
 
-    def _handle_destroy(self):
+    def _handle_destroy(self) -> None:
         self.stop()
-        self._main_window.destroy()
+        if self._main_window:
+            self._main_window.destroy()
         self._root.winfo_toplevel().destroy()
 
     @property
-    def is_active(self):
+    def is_active(self) -> bool:
         """return the information if bar is active or not"""
-        return self._loading_bar and self._loading_bar.is_active
+        return self._loading_bar is not None and self._loading_bar.is_active
 
-    def start(self, interval_ms: Optional[int] = None):
+    def start(self, interval_ms: Optional[int] = None) -> None:
         """start the bar"""
         self._init()
+        if self._loading_bar is None:
+            raise RuntimeError("Cannot start uninitialized bar")
+
         if interval_ms is None:
             self._loading_bar.start()
         else:
             self._loading_bar.start(interval_ms)
         self._locate()
         self._to_top()
 
-    def stop(self):
+    def stop(self) -> None:
         """stop the bar"""
-        self._loading_bar.stop()
-        self._main_window.destroy()
+        if self._loading_bar:
+            self._loading_bar.stop()
+
+        if self._main_window:
+            self._main_window.destroy()
 
+    def update_progress(self, update_by: float = 1.0) -> float:
+        """Same as CircularLoadingBarBase.update_progress"""
+        if self._loading_bar is None:
+            raise RuntimeError("Cannot update uninitialized bar")
+        return self._loading_bar.update_progress(update_by)
 
-def test_spinner_loading_bar(root: Union[tk.Tk, tk.Widget]) -> None:
+
+def test_spinner_loading_bar(root: Union[tk.Tk, tk.Widget]) -> SpinnerLoadingBar:
     """Render a rainbow colored circle spinner bar"""
-    loading = SpinnerLoadingBar(
-        root, colors=SpinnerLoadingBar.RAINBOW,
-    )
+    loading = SpinnerLoadingBar(root, colors=Colors.RAINBOW)
     loading.grid(row=0, column=0)
     loading.start()
 
+    return loading
 
-def test_spinner_sized_loading_bar(root: Union[tk.Tk, tk.Widget]) -> None:
+
+def test_spinner_sized_loading_bar(root: Union[tk.Tk, tk.Widget]) -> SpinnerSizedLoadingBar:
     """Render a spinner bar that the circles resize"""
 
     loading = SpinnerSizedLoadingBar(root)
     loading.grid(row=0, column=1)
     loading.start()
 
+    return loading
+
 
-def test_circular_loading_bar(root: Union[tk.Tk, tk.Widget]) -> None:
+def test_circular_loading_bar(root: Union[tk.Tk, tk.Widget]) -> CircleLoadingBar:
     """Render a circular loading bar"""
     circle_loading_bar = CircleLoadingBar(root, symmetric=True)
     circle_loading_bar.grid(row=0, column=2)
     circle_loading_bar.start(interval_ms=8)
 
+    return circle_loading_bar
+
+
+def test_spinner_loading_bar_with_progress(root: Union[tk.Tk, tk.Widget]) -> SpinnerLoadingBar:
+    """Render a rainbow colored circle spinner bar with a progress"""
+    loading = SpinnerLoadingBar(root, colors=Colors.GRAYED, size=250, progress_options=ProgressOptions(stop_bar_when_max=True))
+    loading.grid(row=1, column=0)
+
+    def _update_progress() -> None:
+        loading.update_progress()
+        if loading.is_active:
+            loading.after(100, _update_progress)
+
+    loading.after(3000, _update_progress)
+    loading.start()
+
+    return loading
+
+
+def test_spinner_sized_loading_bar_with_progress(root: Union[tk.Tk, tk.Widget]) -> SpinnerSizedLoadingBar:
+    """Render a rainbow colored circle spinner bar with a progress"""
+    loading = SpinnerSizedLoadingBar(root, size=250, progress_options=ProgressOptions(stop_bar_when_max=True), colors=Colors.RAINBOW)
+    loading.grid(row=1, column=1)
+
+    def _update_progress() -> None:
+        loading.update_progress()
+        loading.after(100, _update_progress)
+
+    loading.after(3000, _update_progress)
+    loading.start()
+
+    return loading
+
+
+def test_circular_loading_bar_with_progress(root: Union[tk.Tk, tk.Widget]) -> CircleLoadingBar:
+    """Render a rainbow colored circle spinner bar with a progress"""
+    loading = CircleLoadingBar(
+        root, symmetric=True, size=250, progress_options=ProgressOptions(stop_bar_when_max=True), color1="yellow", color2="purple"
+    )
+    loading.grid(row=1, column=2)
+
+    def _update_progress() -> None:
+        loading.update_progress()
+        loading.after(100, _update_progress)
+
+    loading.after(3000, _update_progress)
+    loading.start(interval_ms=8)
+
+    return loading
+
 
 def test_a_working_app() -> None:
     """create an application"""
     root = tk.Tk()
 
     button_frame = tk.Frame(root)
     button_frame.grid()
 
-    def change_bar(kind):
+    text = tk.Text(root)
+    text.insert("1.0", string.ascii_letters * 50)
+    text.grid()
+    spinner = TransparentSpinnerBar(text, SpinnerSizedLoadingBar, size=250)
+
+    def _update_progress() -> None:
+        nonlocal spinner
+
+        spinner.update_progress()
+        root.after(100, _update_progress)
+
+    def change_bar(kind: Type[CircularLoadingBarBase], with_progress: bool = False) -> None:
         nonlocal spinner
         spinner.kind = kind
+        if with_progress:
+            spinner.kwargs["progress_options"] = ProgressOptions(
+                stop_bar_when_max=True, destroy_when_max=True, destroy_callback=spinner.stop
+            )
+        else:
+            try:
+                del spinner.kwargs["progress_options"]
+            except KeyError:
+                pass
 
         spinner.stop()
         if kind == CircleLoadingBar:
             spinner.start(interval_ms=8)
         else:
             spinner.start(interval_ms=100)
 
-    tk.Button(
-        button_frame, text='SpinnerLoadingBar',
-        command=lambda: change_bar(SpinnerLoadingBar)
-    ).grid(row=0, column=0, padx=10, pady=10)
-    tk.Button(
-        button_frame, text='SpinnerSizedLoadingBar',
-        command=lambda: change_bar(SpinnerSizedLoadingBar)
-    ).grid(row=0, column=1, padx=10, pady=10)
-    tk.Button(
-        button_frame, text='CircleLoadingBar',
-        command=lambda: change_bar(CircleLoadingBar)
-    ).grid(row=0, column=2, padx=10, pady=10)
-
-    # pylint:disable=unnecessary-lambda
-    tk.Button(
-        button_frame, text='Stop',
-        command=lambda: spinner.stop()
-    ).grid(row=0, column=3, padx=10, pady=10)
+        if with_progress:
+            root.after(100, _update_progress)
 
-    text = tk.Text(root)
-    text.insert("1.0", string.ascii_letters * 50)
-    text.grid()
+    for idx, options in enumerate((SpinnerLoadingBar, SpinnerSizedLoadingBar, CircleLoadingBar)):
+        tk.Button(
+            button_frame,
+            text=options.__name__,
+            command=lambda opt=options: change_bar(opt),  # type: ignore[misc]
+        ).grid(row=0, column=idx, padx=10, pady=10)
+
+        tk.Button(
+            button_frame,
+            text=options.__name__ + "WithProgress",
+            command=lambda opt=options: change_bar(opt, with_progress=True),  # type: ignore[misc]
+        ).grid(row=1, column=idx, padx=10, pady=10)
+
+    tk.Button(button_frame, text="Stop", command=spinner.stop).grid(row=2, column=1, padx=10, pady=10)
 
-    spinner = TransparentSpinnerBar(
-        text, SpinnerSizedLoadingBar
-    )
     spinner.start()
 
+    def _exit(wait: bool = True) -> None:
+        nonlocal spinner, root
+
+        spinner.stop()
+        if wait:
+            root.after(1000, lambda: _exit(wait=False))
+        else:
+            root.destroy()
+            root.quit()
+
+    root.protocol("WM_DELETE_WINDOW", _exit)
     root.mainloop()
 
 
 def main() -> None:
     """show cases and examples"""
     root = tk.Tk()
 
     test_spinner_loading_bar(root)
-
     test_spinner_sized_loading_bar(root)
-
     test_circular_loading_bar(root)
 
-    test_a_working_app()
+    test_spinner_loading_bar_with_progress(root)
+    test_spinner_sized_loading_bar_with_progress(root)
+    test_circular_loading_bar_with_progress(root)
 
     root.mainloop()
 
+    test_a_working_app()
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `tkhelper-1.0.1/tkhelper/widgets.py` & `tkhelper-2.0.0/tkhelper/widgets.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,123 @@
 """Includes common used tkinter based widgets
 
 Author: Erdogan Onal
 mailto: erdoganonal@windowslive.com
 """
-import os
 import enum
-import string
+import os
 import random
-from typing import Union, Any, Type, Tuple, Callable, Iterable
-
+import string
 import tkinter as tk
-from tkinter import filedialog
-from tkinter import ttk
-from tkinter import font
-from PIL import Image, ImageTk
+from tkinter import filedialog, ttk
+from tkinter.font import Font
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Literal,
+    NoReturn,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    TypeAlias,
+    TypeVar,
+    Union,
+    overload,
+)
 
-from .package_info import __version__, __author__, __mail__
+from PIL import Image, ImageTk
 
 # pylint: disable=too-many-ancestors
+# pylint: disable=too-many-lines
 
 LETTERS_AND_DIGITS = string.ascii_letters + string.digits
-SAMPLES = {}
+SAMPLES: Dict[str, str] = {}
 
 _DOCTEST_TIME_MS = 1 * 1000
+_MAX_WEIGHT = 10000
+
+_T = TypeVar("_T", bound=tk.Widget)
+_GridOptionType: TypeAlias = Dict[str, Union[int, str, Tuple[Union[str, float], Union[str, float]], tk.Misc]]
 
 
-def with_root(function):
+def with_root(function: Callable[..., Any]) -> Callable[..., None]:
     """helper function for docstrings"""
-    def wrapper(*args, **kwargs):
-        timeout = kwargs.pop('timeout', _DOCTEST_TIME_MS)
+
+    def wrapper(*args: Any, **kwargs: Any) -> None:
+        timeout = kwargs.pop("timeout", _DOCTEST_TIME_MS)
         root = tk.Tk()
         function(root, *args, **kwargs)
         root.after(timeout, root.destroy)
         root.mainloop()
+
     return wrapper
 
 
 class TkHelperBaseError(Exception):
     """Base for this module"""
 
 
 class InvalidChoice(TkHelperBaseError):
     """Raise when given choice is not valid"""
 
     def __init__(self, option: Any, options_enum: Any):
-        message = ""\
-            "Given option[{0}] is not a valid option. " \
-            "Valid options: {1}" \
-            "".format(option, ', '.join(map(str, options_enum)))
+        message = f"Given option[{option}] is not a valid option. Valid options: {', '.join(map(str, options_enum))}"
 
         super().__init__(message)
 
 
 class TkRecursionError(TkHelperBaseError, RecursionError):
     """Protection for recursion in resize"""
 
 
 class Objectless(type):
     """A metaclass to disable instantiation"""
 
-    def __call__(cls):
-        raise RuntimeError('{0} should not be instantiated'.format(cls))
+    def __call__(cls, *args: Any, **kwargs: Any) -> NoReturn:
+        raise RuntimeError(f"{cls} should not be instantiated")
 
 
 class WidgetTheme:
     """Theme for a widget. Define configurations to apply.
-        >>> WidgetTheme(bg='black').to_dict()
-        {'bg': 'black'}
+    >>> WidgetTheme(bg='black').to_dict()
+    {'bg': 'black'}
 
-        >>> WidgetTheme(bg='black').keys()
-        dict_keys(['bg'])
+    >>> WidgetTheme(bg='black').keys()
+    dict_keys(['bg'])
     """
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         self.__kwargs = kwargs
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> Dict[str, Any]:
         """Return the dict representation"""
         return dict(self)
 
-    def keys(self) -> Iterable:
+    def keys(self) -> Iterable[str]:
         """Return the keys of the WidgetTheme"""
         return self.__kwargs.keys()
 
-    def __getitem__(self, key: str) -> str:
+    def __getitem__(self, key: str) -> Any:
         """Return the value of the key in the WidgetTheme"""
         return self.__kwargs.get(key)
 
     def __str__(self) -> str:
         return str(self.__kwargs)
 
 
 EMPTY_THEME = WidgetTheme()
 
 
 class Theme(metaclass=Objectless):
     """Base for all themes"""
+
     # For all
     __default__ = EMPTY_THEME
 
     # for root
     ROOT = EMPTY_THEME
 
     # for tk
@@ -140,285 +158,323 @@
     TTK_SIZEGRIP = EMPTY_THEME
     TTK_SPINBOX = EMPTY_THEME
     TTK_TREEVIEW = EMPTY_THEME
 
     @classmethod
     def get_theme(cls, widget_name: str) -> WidgetTheme:
         """return the value of the key"""
-        name = widget_name.lower().replace('::', '_')
+        name = widget_name.lower().replace("::", "_")
         for key in dir(cls):
-            value = getattr(cls, key)
+            value: WidgetTheme = getattr(cls, key)
             if key.lower() == name:
                 return value
-        raise AttributeError(
-            "'{0!r}' object has no attribute '{1}'"
-            "".format(cls, widget_name)
-        )
+        raise AttributeError(f"'{cls!r}' object has no attribute '{widget_name}'")
 
     @classmethod
     def set_theme(cls, key: str, value: WidgetTheme) -> None:
         """set the value of the key"""
         setattr(cls, key.upper(), value)
 
 
 class DarkTheme(Theme):
     """A dark theme"""
+
     __default__ = WidgetTheme(background="#616161")
 
     ROOT = WidgetTheme(background="#616161")
     FRAME = WidgetTheme(background="#616161")
     BUTTON = WidgetTheme(background="#cccccc")
     TEXT = WidgetTheme(background="#757575")
     LABEL = WidgetTheme(background="#757575")
     ENTRY = WidgetTheme()
 
 
 def _configure(widget: Union[tk.Tk, tk.Widget], theme: Type[Theme]) -> None:
     if isinstance(widget, tk.Tk):
-        root_theme = theme.get_theme('root')
+        root_theme = theme.get_theme("root")
         if root_theme is EMPTY_THEME:
             widget.configure(**theme.__default__.to_dict())
         else:
             widget.configure(**root_theme.to_dict())
     elif isinstance(widget, tk.Widget):
         theme_name = widget.widgetName
         widget_theme = theme.get_theme(theme_name)
         if widget_theme is EMPTY_THEME:
-            widget_theme = theme.get_theme('__default__')
+            widget_theme = theme.get_theme("__default__")
 
-        if widget.widgetName.startswith('ttk::'):
+        if widget.widgetName.startswith("ttk::"):
             style = ttk.Style(widget)
             style.configure(widget.winfo_class(), **widget_theme.to_dict())
         else:
             widget.configure(**widget_theme.to_dict())
 
 
-def configure(widget: Union[tk.Tk, tk.Widget], theme: [Theme] = Theme) -> None:
+def configure(widget: Union[tk.Tk, tk.Widget], theme: Type[Theme] = Theme) -> None:
     """Set some configurations for given widget and its children
-        Args:
-            widget: A widget to configure
-            theme:  Apply given theme to the widget.
+    Args:
+        widget: A widget to configure
+        theme:  Apply given theme to the widget.
     """
     _configure(widget, theme)
     for child in widget.winfo_children():
         configure(child, theme)
 
 
 class AddToolTip:
     """Create a tooltip window to display help message
-        Args:
-            widget: A widget to add tooltip
-            text:   Help message to display.
+    Args:
+        widget: A widget to add tooltip
+        text:   Help message to display.
     """
 
     def __init__(self, widget: Union[tk.Tk, tk.Widget], text: str):
         self.text = text
         self.widget = widget
-        self.tip_window = None
+        self.tip_window: Optional[tk.Toplevel] = None
 
-        self.widget.bind('<Enter>', lambda event: self.showtip())
-        self.widget.bind('<Leave>', lambda event: self.hidetip())
+        self.widget.bind("<Enter>", lambda event: self.showtip())
+        self.widget.bind("<Leave>", lambda event: self.hidetip())
 
     def showtip(self) -> None:
         """Display text in tooltip window"""
         x_offset = y_offset = 30
 
         if self.tip_window or not self.text:
             return
-        coord_x, coord_y, _, coord_y2 = self.widget.bbox("insert")
+
+        bbox_result: Tuple[int, int, int, int] = self.widget.bbox("insert")  # type: ignore[call-overload]
+        coord_x, coord_y, _, coord_y2 = bbox_result
         coord_x = coord_x + self.widget.winfo_rootx() + x_offset
         coord_y = coord_y + coord_y2 + self.widget.winfo_rooty() + y_offset
         self.tip_window = tk.Toplevel(self.widget)
         self.tip_window.wm_overrideredirect(True)
-        self.tip_window.wm_geometry("+%d+%d" % (coord_x, coord_y))
-        label = tk.Label(self.tip_window, text=self.text, justify=tk.LEFT,
-                         background="#ffffe0", relief=tk.SOLID, borderwidth=1,
-                         font=("tahoma", "8", "normal"))
+        self.tip_window.wm_geometry(f"+{coord_x}+{coord_y}")
+        label = tk.Label(
+            self.tip_window,
+            text=self.text,
+            justify=tk.LEFT,
+            background="#ffffe0",
+            relief=tk.SOLID,
+            borderwidth=1,
+            font=("tahoma", "8", "normal"),
+        )
         label.pack(ipadx=1)
 
     def hidetip(self) -> None:
         """Hide the tooltip"""
         if self.tip_window:
             self.tip_window.destroy()
 
         self.tip_window = None
 
 
-def create_widget(widget_class: Callable, *args, **kwargs) -> Union[tk.Tk, tk.Widget]:
+def create_widget(widget_class: Type[_T], *args: Any, **kwargs: Any) -> _T:
     """Create a widget with custom properties"""
 
-    tooltip = kwargs.pop('tooltip', None)
+    tooltip = kwargs.pop("tooltip", None)
 
     widget = widget_class(*args, **kwargs)
     if tooltip:
         AddToolTip(widget, tooltip)
 
     return widget
 
 
+def update_and_center(
+    root: tk.Tk | tk.Toplevel, other: tk.Misc | None = None, vertical_taskbar_offset: int = 0, horizontal_taskbar_offset: int = 0
+) -> None:
+    """Update the window and center in the screen"""
+
+    root.update()
+
+    if other:
+        x_pos = other.winfo_rootx() + (other.winfo_width() - root.winfo_width()) // 2
+        y_pos = other.winfo_rooty() + (other.winfo_height() - root.winfo_height()) // 2
+    else:
+        x_pos = (root.winfo_screenwidth() - root.winfo_width() - vertical_taskbar_offset) // 2
+        y_pos = (root.winfo_screenheight() - root.winfo_height() - horizontal_taskbar_offset) // 2
+
+    root.geometry(f"+{x_pos}" f"+{y_pos}")
+
+
 class EntryWithPlaceholder(tk.Entry):
     """Entry widget which allows displaying simple text with a placeholder
-        Args:
-            *args, **kw: Parameters for Entry
-            placeholder: Placeholder for the entry
-            color:       Placeholder background color
-
-        >>> root = tk.Tk()
-        >>> EntryWithPlaceholder(
-        ...     root, placeholder="This is a placeholder"
-        ... ).grid()
-        >>> root.after(_DOCTEST_TIME_MS, root.destroy) # doctest: +ELLIPSIS
-        'after#...'
-        >>> root.mainloop()
+    Args:
+        *args, **kw: Parameters for Entry
+        placeholder: Placeholder for the entry
+        color:       Placeholder background color
+
+    >>> root = tk.Tk()
+    >>> EntryWithPlaceholder(
+    ...     root, placeholder="This is a placeholder"
+    ... ).grid()
+    >>> root.after(_DOCTEST_TIME_MS, root.destroy) # doctest: +ELLIPSIS
+    'after#...'
+    >>> root.mainloop()
     """
 
-    def __init__(self, *args, placeholder: str = "", color: str = 'grey', **kw):
+    def __init__(self, *args: Any, placeholder: str = "", color: str = "grey", **kw: Any):
         super().__init__(*args, **kw)
 
         self._is_empty = True
 
         self.placeholder = placeholder
         self.placeholder_color = color
-        self.default_fg_color = self['fg']
+        self.default_fg_color = self["fg"]
 
         self.__bind("<FocusIn>", self.focus_in)
         self.__bind("<FocusOut>", self.focus_out)
 
         self.put_placeholder()
 
-    def get(self) -> None:
+    def get(self) -> str:
         """Return the text of the entry."""
         if self._is_empty:
-            return None
+            return ""
         return super().get()
 
     def put_placeholder(self) -> None:
         """Put the place holder"""
         self._is_empty = True
         self.insert(0, self.placeholder, placeholder=True)
-        self['fg'] = self.placeholder_color
+        self["fg"] = self.placeholder_color
 
-    def focus_in(self, *_) -> None:
+    def focus_in(self, *_: Any) -> None:
         """Clear placeholder and allow typing"""
         self._is_empty = False
 
-        if self['fg'] == self.placeholder_color:
+        if self["fg"] == self.placeholder_color:
             self.delete(0, tk.END)
-            self['fg'] = self.default_fg_color
+            self["fg"] = self.default_fg_color
 
-    def focus_out(self, *_) -> None:
+    def focus_out(self, *_: Any) -> None:
         """Add placeholder if empty"""
         if not self.get():
             self.put_placeholder()
 
-    def insert(self, *args, **kwargs) -> None:
+    def insert(self, *args: Any, **kwargs: Any) -> None:
         """Insert the text"""
-        placeholder = kwargs.pop('placeholder', False)
-        if not placeholder and self['fg'] == self.placeholder_color:
+        placeholder = kwargs.pop("placeholder", False)
+        if not placeholder and self["fg"] == self.placeholder_color:
             self._is_empty = False
-            self['fg'] = self.default_fg_color
+            self["fg"] = self.default_fg_color
         super().insert(*args, **kwargs)
 
-    def __bind(self, sequence: str = None, func: Callable = None,
-               add: Union[bool, None] = None) -> None:
-        super().bind(sequence, func, add)
-
-    def bind(self, sequence: str = None, func: Callable = None,
-             add: Union[bool, None] = None) -> None:
+    def __bind(
+        self,
+        sequence: Optional[str] = None,
+        func: Optional[Callable[["tk.Event[tk.Misc]"], Any]] = None,
+        add: Optional[Union[bool, Literal["", "+"]]] = None,
+    ) -> str:
+        return super().bind(sequence, func, add)
+
+    def bind(  # type: ignore[override]
+        self,
+        sequence: Optional[str] = None,
+        func: Optional[Callable[["tk.Event[tk.Misc]"], Any]] = None,
+        add: Optional[Union[bool, Literal["", "+"]]] = None,
+    ) -> str:
         """Bind to this widget at event SEQUENCE a call to function FUNC."""
         # Don't allow to override "<FocusIn>" and "<FocusOut>"
         if sequence in ("<FocusIn>", "<FocusOut>"):
-            return
-        self.__bind(sequence, func, add)
+            return sequence
+        return self.__bind(sequence, func, add)
 
-    def unbind(self, sequence: str, funcid: int = None):
+    def unbind(self, sequence: str, funcid: Optional[str] = None) -> None:
         """Unbind for this widget for event SEQUENCE  the
         function identified with FUNC_ID."""
         # Don't allow to delete "<FocusIn>" and "<FocusOut>"
         if sequence in ("<FocusIn>", "<FocusOut>"):
             return
         super().unbind(sequence, funcid)
 
 
 class TargetType(enum.Enum):
     """possible targets"""
+
     FILE = enum.auto()
     FOLDER = enum.auto()
 
 
 class SelectionWidget(tk.Frame):
     """render Entry and Button to enter or select a path
-        Args:
-            master:              Root for the widget.
-            *args
-            **kwargs:            Configurations for base class.
-            placeholder:         Placeholder for entry.
-            entry_options:       Options for the enrty.
-            entry_grid_options:  Grid options for the entry.
-            button_options:      Options for the button.
-            button_grid_options: Grid options for the button.
-            kind:                Type of the selection widget.
-                                 You shall choose a file path or
-                                 folder path.
-            ratio:               Ratio of the entry width over button width
-        >>> # noinspection PyUnresolvedReferences
-        >>> @with_root
-        ... def test_selection_widget(root):
-        ...     SelectionWidget(root, placeholder="1 to 1 ratio.",
-        ...         kind=TargetType.FILE, ratio=(1, 1)).grid()
-        ...     SelectionWidget(root, placeholder="1 to 2 ratio.",
-        ...         kind=TargetType.FILE, ratio=(1, 2)).grid()
-        ...     SelectionWidget(root, placeholder="10 to 1 ratio.",
-        ...         kind=TargetType.FILE, ratio=(10, 1)).grid()
-        ...     SelectionWidget(root, placeholder="10 to 3 ratio.",
-        ...         kind=TargetType.FILE, ratio=(10, 3)).grid()
-        ...     SelectionWidget(root, placeholder="10 to 2 ratio.",
-        ...         kind=TargetType.FILE, ratio=(10, 2)).grid()
-        ...     SelectionWidget(root, placeholder="5 to 1 ratio.",
-        ...         kind=TargetType.FILE, ratio=(5, 1)).grid()
-        >>> test_selection_widget()
+    Args:
+        master:              Root for the widget.
+        *args
+        **kwargs:            Configurations for base class.
+        placeholder:         Placeholder for entry.
+        entry_options:       Options for the entry.
+        entry_grid_options:  Grid options for the entry.
+        button_options:      Options for the button.
+        button_grid_options: Grid options for the button.
+        kind:                Type of the selection widget.
+                             You shall choose a file path or
+                             folder path.
+        ratio:               Ratio of the entry width over button width
+    >>> # noinspection PyUnresolvedReferences
+    >>> @with_root
+    ... def test_selection_widget(root):
+    ...     SelectionWidget(root, placeholder="1 to 1 ratio.",
+    ...         kind=TargetType.FILE, ratio=(1, 1)).grid()
+    ...     SelectionWidget(root, placeholder="1 to 2 ratio.",
+    ...         kind=TargetType.FILE, ratio=(1, 2)).grid()
+    ...     SelectionWidget(root, placeholder="10 to 1 ratio.",
+    ...         kind=TargetType.FILE, ratio=(10, 1)).grid()
+    ...     SelectionWidget(root, placeholder="10 to 3 ratio.",
+    ...         kind=TargetType.FILE, ratio=(10, 3)).grid()
+    ...     SelectionWidget(root, placeholder="10 to 2 ratio.",
+    ...         kind=TargetType.FILE, ratio=(10, 2)).grid()
+    ...     SelectionWidget(root, placeholder="5 to 1 ratio.",
+    ...         kind=TargetType.FILE, ratio=(5, 1)).grid()
+    >>> test_selection_widget()
     """
 
-    def __init__(self, master: Union[tk.Tk, tk.Widget], *args,
-                 placeholder: str = '',
-                 entry_options: dict = None, entry_grid_options: dict = None,
-                 button_options: dict = None, button_grid_options: dict = None,
-                 kind: TargetType = TargetType.FILE,
-                 ratio: Tuple[float, float] = (5, 1),
-                 **kwargs):
+    def __init__(
+        self,
+        master: Union[tk.Tk, tk.Widget],
+        *args: Any,
+        placeholder: str = "",
+        entry_options: Optional[Dict[str, Any]] = None,
+        entry_grid_options: Optional[_GridOptionType] = None,
+        button_options: Optional[Dict[str, Any]] = None,
+        button_grid_options: Optional[_GridOptionType] = None,
+        kind: TargetType = TargetType.FILE,
+        ratio: Tuple[int, int] = (5, 1),
+        **kwargs: Any,
+    ):
         super().__init__(master, *args, **kwargs)
 
         if entry_options is None:
             entry_options = {}
 
         if entry_grid_options is None:
             entry_grid_options = {}
 
         if button_options is None:
             button_options = {}
 
         if button_grid_options is None:
             button_grid_options = {}
 
-        self._entry = None
-        self._button = None
+        self.entry: tk.Entry
+        self.button: tk.Button
 
         self._kind = kind
         self._placeholder = placeholder
 
         # pop items to not override
-        for key in ['row', 'column', 'rowspan', 'columnspan']:
+        for key in ["row", "column", "rowspan", "columnspan"]:
             entry_grid_options.pop(key, None)
             button_grid_options.pop(key, None)
 
         self._place_entry(entry_options, entry_grid_options)
         self._place_button(button_options, button_grid_options)
 
-        self.columnconfigure(0, weight=ratio[0], uniform="foo")
-        self.columnconfigure(1, weight=ratio[1], uniform="foo")
+        self.grid_columnconfigure(0, weight=ratio[0], uniform="foo")
+        self.grid_columnconfigure(1, weight=ratio[1], uniform="foo")
 
     @property
     def kind(self) -> TargetType:
         """return the kind of the select button
 
         >>> # noinspection PyUnresolvedReferences
         >>> @with_root
@@ -476,444 +532,863 @@
             location = filedialog.askdirectory()
         else:
             raise InvalidChoice(self.kind, TargetType)
 
         if location:
             self.text = location
 
-    def _place_entry(self, options: dict, grid_options: dict) -> None:
-        default_options = {
-            'placeholder': self._placeholder
-        }
+    def _place_entry(self, options: Dict[str, Any], grid_options: _GridOptionType) -> None:
+        default_options = {"placeholder": self._placeholder}
         default_options.update(**options)
-        self.entry = create_widget(
-            EntryWithPlaceholder, self, **default_options)
+        self.entry = create_widget(EntryWithPlaceholder, self, **default_options)
 
-        default_grid_options = {
-            'row': 0, 'column': 0,
-            'padx': (0, 5),
-            'sticky': tk.NSEW
+        default_grid_options: _GridOptionType = {
+            "row": 0,
+            "column": 0,
+            "padx": (0, 5),
+            "sticky": tk.NSEW,
         }
         default_grid_options.update(grid_options)
-        self.entry.grid(**default_grid_options)
+        self.entry.grid(None, **default_grid_options)  # type: ignore
 
-    def _place_button(self, options: dict, grid_options: dict) -> None:
-        if 'callback' in options:
-            callback = options.pop('callback')
+    def _place_button(self, options: Dict[str, Any], grid_options: _GridOptionType) -> None:
+        if "callback" in options:
+            callback = options.pop("callback")
 
-            def command():
+            def command() -> Any:
                 return callback(self)
+
         else:
             command = self.command_handler
 
-        default_options = {
-            'text': '...', 'command': command
-        }
+        default_options = {"text": "...", "command": command}
         default_options.update(**options)
         self.button = create_widget(tk.Button, self, **default_options)
 
-        default_grid_options = {
-            'row': 0, 'column': 1,
-            'sticky': tk.NSEW
+        default_grid_options: _GridOptionType = {
+            "row": 0,
+            "column": 1,
+            "sticky": tk.NSEW,
         }
         default_grid_options.update(grid_options)
-        self.button.grid(**default_grid_options)
+        self.button.grid_configure(**default_grid_options)  # type:ignore
 
 
-class _ResizableBase(tk.Widget):
+class MultiColumnListbox:
+    """use a ttk.TreeView as a multicolumn ListBox"""
+
+    def __init__(
+        self,
+        master: tk.Misc,
+        headers: Sequence[str],
+        sort: List[Callable[[Tuple[Any, str]], Any]] | List[bool] | bool | None = None,
+    ) -> None:
+        self.master = master
+        self._headers = list(headers)
+        self._columns: Dict[str, List[str]] = {}
+
+        self._setup_widgets(sort=sort)
+
+    def _setup_widgets(self, sort: List[Callable[[Tuple[Any, str]], Any]] | List[bool] | bool | None = None) -> None:
+        container = ttk.Frame(self.master)
+        container.grid(sticky=tk.NSEW)
+
+        # create a treeview with dual scrollbar
+        self.tree = ttk.Treeview(container, columns=self._headers, show="headings", selectmode=tk.BROWSE)
+        vsb = ttk.Scrollbar(container, orient=tk.VERTICAL, command=self.tree.yview)
+        # hsb = ttk.Scrollbar(orient=tk.HORIZONTAL, command=self.tree.xview)
+
+        self.tree.grid(column=0, row=0, sticky=tk.NSEW, padx=5)
+        vsb.grid(column=1, row=0, sticky=tk.NS)
+
+        self.tree.configure(yscrollcommand=vsb.set)
+        # self.tree.configure(yscrollcommand=hsb.set)
+        # hsb.grid(column=0, row=1, sticky=tk.EW, in_=container)
+        container.grid_columnconfigure(0, weight=_MAX_WEIGHT)
+        container.grid_columnconfigure(1, weight=1)
+        container.grid_rowconfigure(0, weight=1)
+
+        for idx, col in enumerate(self._headers):
+            # adjust the column's width to the header string
+            self.tree.column(col, width=Font().measure(col.title()))
+
+            if (isinstance(sort, bool) and sort) or (isinstance(sort, list) and isinstance(sort[idx], bool) and sort[idx]):
+                self.tree.heading(col, text=col.title(), command=lambda c=col: sortby(self.tree, c, False))  # type: ignore[misc]
+            elif sort is not None and isinstance(sort, list) and callable(sort[idx]):
+                self.tree.heading(
+                    col,
+                    text=col.title(),
+                    command=lambda c=col, sorter=sort[idx]: sortby(self.tree, c, False, sorter=sorter),  # type: ignore[misc]
+                )
+            else:
+                self.tree.heading(col, text=col.title())
+
+    def add_rows(self, columns_list: Sequence[Sequence[str]], smart_width: bool = True) -> List[str]:
+        """Add new rows at the end of the list"""
+        item_ids = []
+        for columns in columns_list:
+            item_id = self.add_row(columns, smart_width=smart_width)
+            item_ids.append(item_id)
+        return item_ids
+
+    def add_row(self, columns: Sequence[str], smart_width: bool = True) -> str:
+        """Add a new row at the end of the list"""
+        return self.insert_row(columns, row=-1, smart_width=smart_width)
+
+    def insert_row(self, columns: Sequence[str], row: int, smart_width: bool = True) -> str:
+        """Add a new row at the end of the list"""
+
+        if len(columns) != len(self._headers):
+            raise ValueError("The length of the columns do not match the length of the headers.")
+
+        item_id = self.tree.insert("", row if row >= 0 else tk.END, values=list(columns))
+
+        if smart_width:
+            for idx, val in enumerate(columns):
+                col_w = Font().measure(val)
+                if self.tree.column(self._headers[idx], width=None) < col_w:  # type: ignore[call-overload]
+                    self.tree.column(self._headers[idx], width=col_w)
+
+        self._columns[item_id] = list(columns)
+        return item_id
+
+    @overload
+    def get_selected(self) -> Optional[Sequence[str]]:
+        pass
+
+    @overload
+    def get_selected(self, key: str) -> Optional[str]:
+        pass
+
+    def get_selected(self, key: Optional[str] = None) -> Sequence[str] | str | None:
+        """return the currently selected item"""
+        selected = self.tree.selection()
+        if len(selected) == 0:
+            return None
+
+        items = self.tree.item(selected[0])["values"]
+        if key is None:
+            return items
+
+        return items[self._headers.index(key)]
+
+    def select_by_column_value(self, column_name: str, column_value: str) -> Optional[str]:
+        """Select the treeview item by column.
+        Selects the first one if multiple values exists.
+        """
+        column_idx = self._headers.index(column_name)
+        item_id: Optional[str] = None
+
+        for key, column_values in self._columns.items():
+            if column_value == column_values[column_idx]:
+                item_id = key
+                break
+
+        if item_id:
+            self.tree.selection_set(item_id)
+            self.tree.focus()
+
+        return item_id
+
+    def select_by_column(self, column: Sequence[str]) -> Optional[str]:
+        """Select the treeview item by column.
+        Selects the first one if multiple values exists.
+        """
+        item_id: Optional[str] = None
+
+        for key, column_values in self._columns.items():
+            if len(column) == len(column_values) and all(l1 == l2 for l1, l2 in zip(column_values, column)):
+                item_id = key
+                break
+
+        if item_id:
+            self.tree.selection_set(item_id)
+            self.tree.focus()
+
+        return item_id
+
+    def clear(self) -> None:
+        """Clear the list"""
+        for item in self._columns:
+            self.tree.delete(item)
+
+        self._columns.clear()
+
+    def destroy(self) -> None:
+        """Clear the list and destroy the widget"""
+
+        self.clear()
+        self._headers.clear()
+        self.tree.master.destroy()
+
 
-    def __init__(self, *args, **kwargs):
-        self._font = None
-        self._width = None
-        self.weight_width = None
-        self.weight_height = None
-        self._dummy_text = None
+def _sorter(item: Tuple[Any, str]) -> Any:
+    try:
+        return int(item[0])
+    except ValueError:
+        return item[0]
+
+
+def sortby(tree: ttk.Treeview, col: int | str, descending: bool, sorter: Callable[[Tuple[Any, str]], Any] = _sorter) -> None:
+    """sort tree contents when a column header is clicked on"""
+    # grab values to sort
+    data = [(tree.set(child, col), child) for child in tree.get_children("")]
+    data.sort(reverse=descending, key=sorter)
+
+    for idx, item in enumerate(data):
+        tree.move(item[1], "", idx)
+    # switch the heading so it will sort in the opposite direction
+    tree.heading(col, command=lambda col=col: sortby(tree, col, not descending))
+
+
+class _ResizableBase(tk.Widget):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        self._font: Font
+        self._width: int = 0
+        self.weight_width: float = 0.0
+        self.weight_height: float = 0.0
+        self._dummy_text: Optional[str] = None
         super().__init__(*args, **kwargs)
 
     def _init(
-            self,
-            weight: Union[float, Tuple[float, float]],
-            base_font: font.Font, resize: bool = True, fix_text_len=None):
+        self,
+        weight: Union[float, Tuple[float, float]],
+        base_font: Font,
+        resize: bool = True,
+        fix_text_len: int = 0,
+    ) -> None:
         """
         A base for resizable widgets.
         """
         self.font = base_font
         try:
-            self.weight_width = float(weight[0])
-            self.weight_height = float(weight[1])
-        except TypeError:
-            self.weight_width = self.weight_height = float(weight)
+            self.weight_width = float(weight[0])  # type: ignore[index]
+            self.weight_height = float(weight[1])  # type: ignore[index]
+        except (TypeError, IndexError):
+            self.weight_width = self.weight_height = float(weight)  # type: ignore[arg-type]
 
         if resize:
             self.winfo_toplevel().bind("<Configure>", self._resize, add="+")
 
         self._dummy_text = ""
         self.fix_text_len = fix_text_len
         self._width = self.winfo_toplevel().winfo_width()
 
     @property
-    def font(self) -> font.Font:
+    def font(self) -> Font:
         """return the font information"""
         return self._font
 
     @font.setter
     def font(self, base_font: Any) -> None:
         """set given font as label font"""
-        if isinstance(base_font, font.Font):
+        if isinstance(base_font, Font):
             self._font = base_font
         else:
             # string fonts are not allowed at this widget
-            raise ValueError("font must be instance of {!r}".format(font.Font))
+            raise ValueError(f"font must be instance of {Font!r}")
 
     @property
-    def fix_text_len(self) -> Union[None, int]:
+    def fix_text_len(self) -> Optional[int]:
         """Return the length of the text which set before is possible"""
+        if self._dummy_text is None:
+            return None
+
         try:
             return len(self._dummy_text)
         except TypeError:
             return None
 
     @fix_text_len.setter
     def fix_text_len(self, value: Union[None, int]) -> None:
         if value is None:
             self._dummy_text = None
             return
         value = int(value)
         try:
             random_sample = SAMPLES[str(value)]
         except KeyError:
-            random_sample = ''.join(random.sample(
-                LETTERS_AND_DIGITS, int(value)))
+            random_sample = "".join(random.sample(LETTERS_AND_DIGITS, int(value)))
             SAMPLES[str(value)] = random_sample
         self._dummy_text = random_sample
 
-    def _resize(self, _) -> None:
+    def _resize(self, _: Any) -> None:
         text = self._dummy_text or self.cget("text")
         if not text:
             return
 
         if self.fix_text_len and len(text) < self.fix_text_len:
-            text += ' ' * (len(text) < self.fix_text_len)
+            text += " " * (len(text) < self.fix_text_len)
 
         top_level_width = self.winfo_toplevel().winfo_width()
         if top_level_width == 1:
             # If width equals to 1 means that
             # the main window is in initial step.
             return
 
         expected_width = top_level_width * self.weight_width
         dummy_font = self.font.copy()
 
         while True:
             current_width = dummy_font.measure(text)
-            font_size = dummy_font.actual('size')
+            font_size = dummy_font.actual("size")
 
             if current_width < expected_width:
                 # if current width smaller than expected
                 # increase the dummy font size by one
-                dummy_font['size'] = font_size + 1
+                dummy_font["size"] = font_size + 1
                 if dummy_font.measure(text) > expected_width:
                     # if increasing size exceeds the expected,
                     # undo increasing and exit the loop
-                    dummy_font['size'] = font_size
+                    dummy_font["size"] = font_size
                     break
                 # still have spaces, so continue
             else:
                 # if current width grater than expected
                 # decrease the dummy font size by one
-                dummy_font['size'] = font_size - 1
+                dummy_font["size"] = font_size - 1
                 if dummy_font.measure(text) < expected_width:
                     # if it is fit, break the loop
                     break
                 # if it is not fit, means we have spaces
                 # so, continue
 
         self.font = dummy_font
-        self.configure(font=self.font)
+        self.configure(font=self.font)  # type: ignore[call-arg]
 
 
 class ResizableLabel(tk.Label, _ResizableBase):
     """Create a label which resize with outer window
-        Args:
-            master:         Root of the widget.
-            *args
-            **kwargs:     Configurations for base class.
-            weight:       The ratio of the label width over top level width.
-                          The calculation will be based on the text of the label.
-            resize:       If True, the widget wile be resized with top level window.
-            fix_text_len: If passed, the label ignores its actual text and uses a dummy
-                          text with length of this value. This feature allows you to
-                          keep fixed size the label. Basically, whatever the text size is,
-                          the label size will not change.
-
-        >>> timeout = 1
-        >>> # noinspection PyUnresolvedReferences
-        >>> @with_root
-        ... def resizable_label_test(root):
-        ...     root.geometry("500x500")
-        ...     tk.Label(root,
-        ...         text="Default tk.Label - Click X to close. Timeout is {0} secs."
-        ...         "".format(timeout)
-        ...     ).grid()
-        ...     ResizableLabel(root, weight=0.5,
-        ...         text="This text covers 50% of the total width.").grid()
-        ...     ResizableLabel(root, weight=1,
-        ...         text="This text covers 100% of the total width.").grid()
-        ...     ResizableLabel(root, weight=1, resize=False,
-        ...         text="This text covers 100% of the total width. Non resizable!"
-        ...     ).grid()
-        ...     ResizableLabel(root, weight=.3, fix_text_len=20,
-        ...         text="This text covers 50% of the total width. fix_text_len is 20"
-        ...     ).grid()
-        >>> resizable_label_test(timeout=timeout * 1000)
+    Args:
+        master:         Root of the widget.
+        *args
+        **kwargs:     Configurations for base class.
+        weight:       The ratio of the label width over top level width.
+                      The calculation will be based on the text of the label.
+        resize:       If True, the widget wile be resized with top level window.
+        fix_text_len: If passed, the label ignores its actual text and uses a dummy
+                      text with length of this value. This feature allows you to
+                      keep fixed size the label. Basically, whatever the text size is,
+                      the label size will not change.
+
+    >>> timeout = 1
+    >>> # noinspection PyUnresolvedReferences
+    >>> @with_root
+    ... def resizable_label_test(root):
+    ...     root.geometry("500x500")
+    ...     tk.Label(root,
+    ...         text="Default tk.Label - Click X to close. Timeout is {0} secs."
+    ...         "".format(timeout)
+    ...     ).grid()
+    ...     ResizableLabel(root, weight=0.5,
+    ...         text="This text covers 50% of the total width.").grid()
+    ...     ResizableLabel(root, weight=1,
+    ...         text="This text covers 100% of the total width.").grid()
+    ...     ResizableLabel(root, weight=1, resize=False,
+    ...         text="This text covers 100% of the total width. Non resizable!"
+    ...     ).grid()
+    ...     ResizableLabel(root, weight=.3, fix_text_len=20,
+    ...         text="This text covers 50% of the total width. fix_text_len is 20"
+    ...     ).grid()
+    >>> resizable_label_test(timeout=timeout * 1000)
 
     """
 
-    def __init__(self,
-                 master: Union[tk.Tk, tk.Widget],
-                 *args, weight: float = 1.0, resize: bool = True,
-                 fix_text_len: Union[int, None] = None, **kwargs):
-        base_font = kwargs.pop('font', font.Font())
+    def __init__(
+        self,
+        master: Union[tk.Tk, tk.Widget],
+        *args: Any,
+        weight: float = 1.0,
+        resize: bool = True,
+        fix_text_len: int = 0,
+        **kwargs: Any,
+    ):
+        base_font = kwargs.pop("font", Font())
 
         super().__init__(master, *args, **kwargs)
         self._init(weight, base_font, resize, fix_text_len)
 
-    def configure(self, cnf: Any = None, **kwargs) -> None:
+    def configure(self, cnf: Any = None, **kwargs: Any) -> None:  # type: ignore[override]
         """override the configure method to capture font"""
-        self.font = kwargs.get('font', font.Font())
+        self.font = kwargs.get("font", Font())
         super().configure(cnf, **kwargs)
 
 
 class ResizableLabelImage(ResizableLabel):
     """A label which can resize
-        Args:
-            *args
-            **kwargs:   Configurations for base class.
-            image:      The image to display on the screen.
-            image_path: The path of the image.
+    Args:
+        *args
+        **kwargs:   Configurations for base class.
+        image:      The image to display on the screen.
+        image_path: The path of the image.
     """
 
-    def __init__(self, *args,
-                 image: Image.Image = None,
-                 image_path: str = None, **kwargs):
+    @overload
+    def __init__(self, *args: Any, image: Image.Image, **kwargs: Any) -> None:
+        pass
+
+    @overload
+    def __init__(self, *args: Any, image_path: str, **kwargs: Any) -> None:
+        pass
+
+    def __init__(
+        self,
+        *args: Any,
+        image: Optional[Image.Image] = None,
+        image_path: Optional[str] = None,
+        **kwargs: Any,
+    ) -> None:
         if image is not None and image_path is not None:
-            raise ValueError(
-                "you are allowed to pass only image or image_path"
-            )
+            raise ValueError("you are allowed to pass only image or image_path")
+
+        self._original: Image.Image
 
         if image:
             self._original = image
-        if image_path:
+        elif image_path:
             self._original = Image.open(image_path)
-        self._resized = None
+        self._resized: Optional[ImageTk.PhotoImage] = None
 
         super().__init__(*args, **kwargs, image=self._resized)
 
-    def _resize(self, _) -> None:
+    def _resize(self, _: Any) -> None:
         min_size = 10
         width = self.winfo_toplevel().winfo_width()
         height = self.winfo_toplevel().winfo_height()
         size = min(
             max(int(width * self.weight_width), min_size),
-            max(int(height * self.weight_height), min_size)
+            max(int(height * self.weight_height), min_size),
         )
 
         self.set_image(self._original, (size, size))
 
-    def set_image(self, image: Image.Image,
-                  image_size: Tuple[int, int] = None,
-                  resample: int = Image.ANTIALIAS):
+    def set_image(
+        self,
+        image: Image.Image,
+        image_size: Optional[Tuple[int, int]] = None,
+        resample: Literal[0, 1, 2, 3, 4, 5] = Image.Resampling.LANCZOS,  # type: ignore[assignment]
+    ) -> None:
         """Set the given image"""
         self._original = image
 
         if image_size is None:
             resized = image
         else:
             resized = image.resize(image_size, resample)
         self._resized = ImageTk.PhotoImage(resized)
 
         self.configure(image=self._resized)
 
 
 class ResizableButton(tk.Button, _ResizableBase):
     """Create a button which resize with outer window
-        Args:
-            master:         Root of the widget.
-            *args
-            **kwargs:       Configurations for base class.
-            weight:         The ratio of the button width over top level width.
-                            The calculation will be based on the text of the button.
-            resize:         If True, the widget wile be resized with top level window.
-            fixed_text_len: If passed, the button ignores its actual text and uses a dummy
-                            text with length of this value. This feature allows you to
-                            keep fixed size the button. Basically, whatever the text size is,
-                            the button size will not change.
-
-        >>> timeout = 1
-        >>> # noinspection PyUnresolvedReferences
-        >>> @with_root
-        ... def resizable_button_test(root):
-        ...     root.geometry("500x500")
-        ...     tk.Button(root,
-        ...         text="Default tk.Button - Click X to close. Timeout is {0} secs."
-        ...         "".format(timeout)
-        ...     ).grid()
-        ...     ResizableButton(root, weight=0.5,
-        ...         text="This text covers 50% of the total width.").grid()
-        ...     ResizableButton(root, weight=1,
-        ...         text="This text covers 100% of the total width.").grid()
-        ...     ResizableButton(root, weight=1, resize=False,
-        ...         text="This text covers 100% of the total width. Non resizable!"
-        ...     ).grid()
-        ...     ResizableButton(root, weight=.3, fix_text_len=20,
-        ...         text="This text covers 50% of the total width. fix_text_len is 20"
-        ...     ).grid()
-        >>> resizable_button_test(timeout=timeout * 1000)
+    Args:
+        master:         Root of the widget.
+        *args
+        **kwargs:       Configurations for base class.
+        weight:         The ratio of the button width over top level width.
+                        The calculation will be based on the text of the button.
+        resize:         If True, the widget wile be resized with top level window.
+        fixed_text_len: If passed, the button ignores its actual text and uses a dummy
+                        text with length of this value. This feature allows you to
+                        keep fixed size the button. Basically, whatever the text size is,
+                        the button size will not change.
+
+    >>> timeout = 1
+    >>> # noinspection PyUnresolvedReferences
+    >>> @with_root
+    ... def resizable_button_test(root):
+    ...     root.geometry("500x500")
+    ...     tk.Button(root,
+    ...         text="Default tk.Button - Click X to close. Timeout is {0} secs."
+    ...         "".format(timeout)
+    ...     ).grid()
+    ...     ResizableButton(root, weight=0.5,
+    ...         text="This text covers 50% of the total width.").grid()
+    ...     ResizableButton(root, weight=1,
+    ...         text="This text covers 100% of the total width.").grid()
+    ...     ResizableButton(root, weight=1, resize=False,
+    ...         text="This text covers 100% of the total width. Non resizable!"
+    ...     ).grid()
+    ...     ResizableButton(root, weight=.3, fix_text_len=20,
+    ...         text="This text covers 50% of the total width. fix_text_len is 20"
+    ...     ).grid()
+    >>> resizable_button_test(timeout=timeout * 1000)
     """
 
-    def __init__(self,
-                 master: Union[tk.Tk, tk.Widget],
-                 *args, weight: float = 1.0,
-                 resize: bool = True,
-                 fix_text_len: int = None, **kwargs):
-        self._font = None
-        base_font = kwargs.pop('font', font.Font())
+    def __init__(
+        self,
+        master: Union[tk.Tk, tk.Widget],
+        *args: Any,
+        weight: float = 1.0,
+        resize: bool = True,
+        fix_text_len: int = 0,
+        **kwargs: Any,
+    ):
+        self._font: Font
+        base_font = kwargs.pop("font", Font())
 
         super().__init__(master, *args, **kwargs)
         self._init(weight, base_font, resize, fix_text_len)
 
-    def configure(self, cnf: Any = None, **kwargs) -> None:
+    def configure(  # type: ignore[override]
+        self, cnf: Dict[str, Any] | None = None, **kwargs: Any
+    ) -> Optional[Dict[str, Tuple[str, str, str, Any, Any]]]:
         """override the configure method to capture font"""
-        self.font = kwargs.get('font', font.Font())
-        super().configure(cnf, **kwargs)
+        self.font = kwargs.get("font", Font())
+        return super().configure(cnf, **kwargs)
 
 
 class FixedSizedOptionMenu(ttk.OptionMenu):
     """A fix-sized option menu, calculates the width from options and placeholder
-        Args:
-            master:      Root of the widget.
-            variable:    Tkinter variable for dropdown menu.
-            *values:     Options for dropdown menu.
-            placeholder: Help-like option. Cannot be selected as a value.
-            **kwargs:    Configurations for base class.
-
-        >>> timeout = 1
-        >>> # noinspection PyUnresolvedReferences
-        >>> @with_root
-        ... def fixed_sized_option_menu(root):
-        ...     variable = tk.StringVar()
-        ...     options = ["option1", "option2", "option3 with a long name"]
-        ...     FixedSizedOptionMenu(
-        ...         root, variable, *options,
-        ...         placeholder="This is the placeholder"
-        ...     ).grid()
-        >>> fixed_sized_option_menu(timeout=timeout * 1000)
+    Args:
+        master:      Root of the widget.
+        variable:    Tkinter variable for dropdown menu.
+        *values:     Options for dropdown menu.
+        placeholder: Help-like option. Cannot be selected as a value.
+        **kwargs:    Configurations for base class.
+
+    >>> timeout = 1
+    >>> # noinspection PyUnresolvedReferences
+    >>> @with_root
+    ... def fixed_sized_option_menu(root):
+    ...     variable = tk.StringVar()
+    ...     options = ["option1", "option2", "option3 with a long name"]
+    ...     FixedSizedOptionMenu(
+    ...         root, variable, *options,
+    ...         placeholder="This is the placeholder"
+    ...     ).grid()
+    >>> fixed_sized_option_menu(timeout=timeout * 1000)
     """
 
-    def __init__(self,
-                 master: Union[tk.Tk, tk.Widget],
-                 variable: tk.Variable, *values,
-                 placeholder: str = None, **kwargs):
-
+    def __init__(
+        self,
+        master: Union[tk.Tk, tk.Widget],
+        variable: tk.StringVar,
+        *values: str,
+        placeholder: Optional[str] = None,
+        **kwargs: Any,
+    ):
         self._placeholder = placeholder
         if placeholder is None:
             placeholder = values[0]
         super().__init__(master, variable, placeholder, *values, **kwargs)
+        self._variable = variable
         self.configure(**self._get_option_menu_style(placeholder, values))
 
     def get(self) -> Union[str, None]:
         """Return the value of drop down menu. None will be returned
         if no option is selected and placeholder exist.
         """
         value = self._variable.get()
         if value == self._placeholder:
             return None
         return value
 
     @staticmethod
-    def _get_option_menu_style(placeholder: str, option_list: Iterable) -> dict:
+    def _get_option_menu_style(placeholder: str, option_list: Iterable[str]) -> Dict[str, Any]:
         style = {}
-        width = max([len(i) for i in option_list])
+        width = max((len(i) for i in option_list))
         width = max(len(placeholder), width)
 
         style["width"] = int(width) + 2  # add some offset
 
         return style
 
 
+# pylint: disable=too-many-arguments
+class VerticalScrollFrame(ttk.Frame):
+    """A widget container with a vertical scrollbar."""
+
+    def __init__(
+        self,
+        master: tk.Misc,
+        padding: int = 2,
+        autohide: bool = False,
+        height: int = 200,
+        width: int = 300,
+        scrollheight: float = None,  # type: ignore[assignment]
+        **kwargs: Any,
+    ):
+        # content frame container
+        self.container = ttk.Frame(master=master, relief=tk.FLAT, borderwidth=0, width=width, height=height)
+        self.container.bind("<Configure>", lambda _: self.yview())
+        self.container.propagate(False)
+
+        # content frame
+        super().__init__(master=self.container, padding=padding, **kwargs)
+        self.place(rely=0.0, relwidth=1.0, height=scrollheight)
+
+        # vertical scrollbar
+        self.vscroll = ttk.Scrollbar(master=self.container, command=self.yview, orient=tk.VERTICAL)
+        self.show_scrollbars()
+
+        self.winsys: str = self.tk.call("tk", "windowingsystem")
+
+        # setup autohide scrollbar
+        self.autohide = autohide
+        if self.autohide:
+            self.hide_scrollbars()
+
+        # widget event binding
+        self.container.bind("<Enter>", self._on_enter, "+")
+        self.container.bind("<Leave>", self._on_leave, "+")
+        self.container.bind("<Map>", self._on_map, "+")
+        self.bind("<<MapChild>>", self._on_map_child, "+")
+
+        self.bind_all("<MouseWheel>", self.scroll_event, add=True)
+
+        # delegate content geometry methods to container frame
+        _methods = vars(tk.Pack).keys() | vars(tk.Grid).keys() | vars(tk.Place).keys()
+        for method in _methods:
+            if any(["pack" in method, "grid" in method, "place" in method]):
+                # prefix content frame methods with 'content_'
+                setattr(self, f"content_{method}", getattr(self, method))
+                # overwrite content frame methods from container frame
+                setattr(self, method, getattr(self.container, method))
+
+    def yview(self, *args: Any) -> None:
+        """Update the vertical position of the content frame within the container."""
+
+        if not args:
+            first, _ = self.vscroll.get()  # type: ignore[misc]
+            self.yview_moveto(fraction=first)
+        elif args[0] == "moveto":
+            self.yview_moveto(fraction=float(args[1]))
+        elif args[0] == "scroll":
+            self.yview_scroll(number=int(args[1]), what=args[2])
+        else:
+            return
+
+    def yview_moveto(self, fraction: float) -> None:
+        """Update the vertical position of the content frame within the container.
+
+        fraction (float):
+                The relative position of the content frame within the container.
+        """
+        base, thumb = self._measures()
+        if fraction < 0:
+            first = 0.0
+        elif (fraction + thumb) > 1:
+            first = 1 - thumb
+        else:
+            first = fraction
+        self.vscroll.set(first, first + thumb)
+        self.content_place(rely=-first * base)  # type: ignore[attr-defined]  # pylint: disable=no-member
+
+    def yview_scroll(self, number: int, what: str) -> None:  # pylint: disable=unused-argument
+        """Update the vertical position of the content frame within the container.
+
+        number (int):
+            The amount by which the content frame will be moved within the container frame by 'what' units.
+        what (str):
+            The type of units by which the number is to be interpreted. This parameter is currently not used and is assumed to be 'units'.
+        """
+        first, _ = self.vscroll.get()  # type: ignore[misc]
+        fraction = (number / 100) + first
+        self.yview_moveto(fraction)
+
+    def scroll_top(self) -> None:
+        """Go to the top of the widget"""
+        self.yview_moveto(0.0)
+
+    def scroll_bottom(self) -> None:
+        """Go to the bottom of the widget"""
+        self.yview_moveto(1.0)
+
+    @staticmethod
+    def _get_parent(widget: tk.Misc) -> Optional[ttk.Frame]:
+        while widget.master:
+            widget = widget.master
+            if isinstance(widget, ttk.Frame):
+                return widget
+
+        return None
+
+    def _has_same_widget(self, widget: tk.Misc) -> bool:
+        try:
+            if widget.winfo_toplevel() is not self.winfo_toplevel():
+                raise tk.TclError
+        except tk.TclError:
+            return False
+
+        while widget:
+            if self is widget:
+                return True
+            widget = self._get_parent(widget)  # type: ignore[assignment]
+
+        return widget is not None
+
+    def scroll_event(self, event: "tk.Event[tk.Misc]") -> None:
+        """Allow to scroll with mouse"""
+        if not self._has_same_widget(event.widget):
+            return
+        number = -1 * (event.delta // 120)
+        self.yview_scroll(number, tk.UNITS)
+
+    def enable_scrolling(self) -> None:
+        """Enable mousewheel scrolling on the frame and all of its children."""
+        widgets: Iterable[tk.Widget] = [self, *self.winfo_children()]
+        for widget in widgets:
+            bindings = widget.bind()
+            if self.winsys.lower() == "x11":
+                if "<Button-4>" in bindings or "<Button-5>" in bindings:
+                    continue
+                widget.bind("<Button-4>", self._on_mousewheel, "+")
+                widget.bind("<Button-5>", self._on_mousewheel, "+")
+            else:
+                if "<MouseWheel>" not in bindings:
+                    widget.bind("<MouseWheel>", self._on_mousewheel, "+")
+
+    def disable_scrolling(self) -> None:
+        """Disable mousewheel scrolling on the frame and all of its children."""
+        widgets: Iterable[tk.Widget] = [self, *self.winfo_children()]
+        for widget in widgets:
+            if self.winsys.lower() == "x11":
+                widget.unbind("<Button-4>")
+                widget.unbind("<Button-5>")
+            else:
+                widget.unbind("<MouseWheel>")
+
+    def hide_scrollbars(self) -> None:
+        """Hide the scrollbars."""
+        self.vscroll.pack_forget()
+
+    def show_scrollbars(self) -> None:
+        """Show the scrollbars."""
+        self.vscroll.pack(side=tk.RIGHT, fill=tk.Y)
+
+    def autohide_scrollbar(self) -> None:
+        """Toggle the autohide functionality. Show the scrollbars when
+        the mouse enters the widget frame, and hide when it leaves the
+        frame."""
+        self.autohide = not self.autohide
+
+    def _measures(self) -> Tuple[float, float]:
+        """Measure the base size of the container and the thumb size
+        for use in the yview methods"""
+        outer = self.container.winfo_height()
+        inner = max([self.winfo_height(), outer])
+        base = inner / outer
+        if inner == outer:
+            thumb = 1.0
+        else:
+            thumb = outer / inner
+        return base, thumb
+
+    def _on_map_child(self, _: "tk.Event[Any]") -> None:
+        """Callback for when a widget is mapped to the content frame."""
+        if self.container.winfo_ismapped():
+            self.yview()
+
+    def _on_enter(self, _: "tk.Event[Any]") -> None:
+        """Callback for when the mouse enters the widget."""
+        self.enable_scrolling()
+        if self.autohide:
+            self.show_scrollbars()
+
+    def _on_leave(self, _: "tk.Event[Any]") -> None:
+        """Callback for when the mouse leaves the widget."""
+        self.disable_scrolling()
+        if self.autohide:
+            self.hide_scrollbars()
+
+    def _on_configure(self, _: "tk.Event[Any]") -> None:
+        """Callback for when the widget is configured"""
+        self.yview()
+
+    def _on_map(self, _: "tk.Event[Any]") -> None:
+        self.yview()
+
+    def _on_mousewheel(self, event: "tk.Event[Any]") -> None:
+        """Callback for when the mouse wheel is scrolled."""
+        if self.winsys.lower() == "win32":
+            delta = -int(event.delta / 120)
+        elif self.winsys.lower() == "aqua":
+            delta = -event.delta
+        elif event.num == 4:
+            delta = -10
+        elif event.num == 5:
+            delta = 10
+        self.yview_scroll(delta, tk.UNITS)
+
+
 def test_selection(root: Union[tk.Tk, tk.Widget]) -> None:
     """test for SelectionWidget"""
     counter = 0
 
-    def callback(self):
+    def callback(self: SelectionWidget) -> None:
         nonlocal counter
         counter += 1
-        self.text = "You click {0} times".format(counter)
+        self.text = f"You click {counter} times"
 
     selection = SelectionWidget(
-        root, placeholder='put the placeholder here',
-        entry_options={'tooltip': 'You may add a help here'},
-        entry_grid_options={'padx': 5, 'pady': 5},
+        root,
+        placeholder="put the placeholder here",
+        entry_options={"tooltip": "You may add a help here"},
+        entry_grid_options={"padx": 5, "pady": 5},
         button_options={
-            'callback': callback, 'text': u'\u25A9',
-            'tooltip': 'Click the button to increase counter'
+            "callback": callback,
+            "text": "\u25A9",
+            "tooltip": "Click the button to increase counter",
         },
-        button_grid_options={'padx': 5, 'pady': 5},
+        button_grid_options={"padx": 5, "pady": 5},
     )
     selection.grid()
 
-    SelectionWidget(root, placeholder='Default settings').grid()
+    SelectionWidget(root, placeholder="Default settings").grid()
 
 
 def test_resizable_label(root: Union[tk.Tk, tk.Widget]) -> None:
     """test for ResizableLabel"""
     label_frame = tk.Frame(root)
     label_frame.grid()
 
     ResizableLabel(
-        label_frame, text='initial', weight=0.2,
+        label_frame,
+        text="initial",
+        weight=0.2,
     ).grid(row=0, column=0)
 
     ResizableLabel(
-        label_frame, weight=0.6,
+        label_frame,
+        weight=0.6,
         text="This is expandable label",
     ).grid(row=0, column=1)
 
     ResizableLabel(
-        label_frame, text='end', weight=0.2,
+        label_frame,
+        text="end",
+        weight=0.2,
     ).grid(row=0, column=2)
 
 
 def test_resizable_label_image(root: Union[tk.Tk, tk.Widget]) -> None:
     """Resizable image test"""
     default_image_path = os.path.join(os.getcwd(), "test.png")
     if not os.path.isfile(default_image_path):
         # If no image found, skip the test
         return
     image_frame = tk.Frame(root)
     image_frame.grid()
 
-    ResizableLabelImage(
-        image_frame, weight=(0.4, 0.4),
-        image_path=default_image_path
-    ).grid(row=0, column=0, sticky=tk.NSEW)
+    ResizableLabelImage(image_frame, weight=(0.4, 0.4), image_path=default_image_path).grid(row=0, column=0, sticky=tk.NSEW)
 
-    ResizableLabelImage(
-        image_frame, weight=(0.4, 0.4),
-        image=Image.open(default_image_path)
-    ).grid(row=0, column=1, sticky=tk.NSEW)
+    ResizableLabelImage(image_frame, weight=(0.4, 0.4), image=Image.open(default_image_path)).grid(row=0, column=1, sticky=tk.NSEW)
 
 
 def test_resizable_button(root: Union[tk.Tk, tk.Widget]) -> None:
     """Resizable button test"""
     button_frame = tk.Frame(root)
     button_frame.grid()
 
     ResizableButton(
-        button_frame, text='test', weight=0.1,
+        button_frame,
+        text="test",
+        weight=0.1,
     ).grid(row=0, column=0, sticky=tk.NSEW)
 
 
 def test() -> None:
     """the module test"""
     root = tk.Tk()
```

