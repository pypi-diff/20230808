# Comparing `tmp/anydyce-0.4.3-py3-none-any.whl.zip` & `tmp/anydyce-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 22064 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1013 b- defN 23-Aug-07 11:44 anydyce/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 23-Aug-07 11:45 anydyce/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 11:44 anydyce/py.typed
--rw-r--r--  2.0 unx    62524 b- defN 23-Aug-07 11:44 anydyce/viz.py
--rw-r--r--  2.0 unx     2118 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    15588 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      678 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/RECORD
-9 files, 82069 bytes uncompressed, 20904 bytes compressed:  74.5%
+Zip file size: 22447 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1013 b- defN 23-Aug-07 23:17 anydyce/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-07 23:18 anydyce/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 23:17 anydyce/py.typed
+-rw-r--r--  2.0 unx    64353 b- defN 23-Aug-07 23:17 anydyce/viz.py
+-rw-r--r--  2.0 unx     2118 b- defN 23-Aug-07 23:18 anydyce-0.4.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15588 b- defN 23-Aug-07 23:18 anydyce-0.4.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 23:18 anydyce-0.4.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-07 23:18 anydyce-0.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      678 b- defN 23-Aug-07 23:18 anydyce-0.4.4.dist-info/RECORD
+9 files, 83898 bytes uncompressed, 21287 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: anydyce/py.typed
 Comment: 
 
 Filename: anydyce/viz.py
 Comment: 
 
-Filename: anydyce-0.4.3.dist-info/LICENSE
+Filename: anydyce-0.4.4.dist-info/LICENSE
 Comment: 
 
-Filename: anydyce-0.4.3.dist-info/METADATA
+Filename: anydyce-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: anydyce-0.4.3.dist-info/WHEEL
+Filename: anydyce-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: anydyce-0.4.3.dist-info/top_level.txt
+Filename: anydyce-0.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: anydyce-0.4.3.dist-info/RECORD
+Filename: anydyce-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anydyce/_version.py

```diff
@@ -1,3 +1,3 @@
-__vers_str__ = "0.4.3"
-__version__ = (0, 4, 3)
+__vers_str__ = "0.4.4"
+__version__ = (0, 4, 4)
```

## anydyce/viz.py

```diff
@@ -85,35 +85,38 @@
     alpha: float
     burst_cmap_inner: str
     burst_cmap_link: bool
     burst_cmap_outer: str
     burst_color_bg: str
     burst_color_bg_trnsp: bool
     burst_color_text: str
+    burst_columns: int
     burst_swap: bool
     burst_zero_fill_normalize: bool
     enable_cutoff: bool
     graph_type: TraditionalPlotType
     img_type: ImageType
     markers: str
     plot_style: str
-    scale: int
+    resolution: int
     show_shadow: bool
 
 
 # ---- Data ----------------------------------------------------------------------------
 
 
 DEFAULT_ALPHA = 0.75
 DEFAULT_CMAP_BURST_INNER = "RdYlGn_r"
 DEFAULT_CMAP_BURST_OUTER = "RdYlBu_r"
 DEFAULT_COLOR_TEXT = "black"
 DEFAULT_COLOR_BG = "white"
+DEFAULT_COLS_BURST = 3
 DEFAULT_MARKERS = "oX^v><dP"
 DEFAULT_PLOT_STYLE = "bmh"
+DEFAULT_RESOLUTION = 12
 _LABEL_LIM = Fraction(1, 2**5)
 _CUTOFF_BASE = 10
 _CUTOFF_EXP = 6
 
 
 _MARKERS = {
     "point": ".",
@@ -302,25 +305,25 @@
         default_factory=partial(
             widgets.Checkbox,
             description="Hide Small Outcomes",
         ),
     )
 
     # Generic display widgets
-    scale: widgets.FloatLogSlider = field(
+    resolution: widgets.IntSlider = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.IntSlider,
-            value=12,
-            min=8,
-            max=16,
+            value=DEFAULT_RESOLUTION,
+            min=4,
+            max=32,
             step=1,
             continuous_update=False,
-            description="Scale",
+            description="Resolution",
         ),
     )
 
     img_type: widgets.ToggleButtons = field(
         init=False,
         repr=False,
         default_factory=partial(
@@ -365,15 +368,15 @@
     )
 
     burst_color_bg: widgets.ColorPicker = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.ColorPicker,
-            value="white",
+            value=DEFAULT_COLOR_BG,
             # options=sorted(sorted(matplotlib.colors.CSS4_COLORS.keys())),
             concise=False,
             description="Background",
         ),
     )
 
     burst_color_bg_trnsp: widgets.Checkbox = field(
@@ -387,21 +390,35 @@
     )
 
     burst_color_text: widgets.ColorPicker = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.ColorPicker,
-            value="black",
+            value=DEFAULT_COLOR_TEXT,
             # options=sorted(sorted(matplotlib.colors.CSS4_COLORS.keys())),
             concise=False,
             description="Text",
         ),
     )
 
+    burst_columns: widgets.IntSlider = field(
+        init=False,
+        repr=False,
+        default_factory=partial(
+            widgets.IntSlider,
+            value=DEFAULT_COLS_BURST,
+            min=1,
+            max=12,
+            step=1,
+            continuous_update=False,
+            description="Columns",
+        ),
+    )
+
     burst_swap: widgets.Checkbox = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.Checkbox,
             description="Swap Inner/Outer Histograms",
             disabled=True,
@@ -448,15 +465,15 @@
     )
 
     markers: widgets.Text = field(
         init=False,
         repr=False,
         default_factory=partial(
             widgets.Text,
-            value=" ",
+            value=DEFAULT_MARKERS,
             description="Markers",
         ),
     )
 
     plot_style: widgets.Dropdown = field(
         init=False,
         repr=False,
@@ -510,14 +527,17 @@
 
     - *initial_burst_color_bg_trnsp* is the initially selected background transparency
        color burst graphs (defaults to ``#!python False``).
 
     - *initial_burst_color_text* is the initially selected text color for burst graphs
        (defaults to ``#!python "black"``).
 
+    - *initial_burst_columns* is the initially selected number of columns for displaying
+       burst graphs (defaults to ``#!python 3``).
+
     - *initial_burst_swap* is whether the inner and outer burst graphs should be swapped
        at first (defaults to ``#!python False``).
 
     - *initial_burst_zero_fill_normalize* is whether all burst graphs should share a
        scale at first (i.e., so similar values share similar colors across burst graphs)
        (defaults to ``#!python False``).
 
@@ -534,34 +554,39 @@
        (defaults to ``#!python "oX^v><dP"``).
 
     - *initial_plot_style* is the starting color style for non-burst graphs (defaults to
        ``#!python "bmh"``).
 
     - *initial_show_shadow* is whether shadows should be shown for non-burst graphs at
        first (defaults to ``#!python False``).
+
+    - *initial_resolution* is the starting value for the graph resolution (defaults to
+      ``#!python 12``).
     """
 
     @beartype
     def __init__(
         self,
         *,
         initial_alpha: float = DEFAULT_ALPHA,
         initial_burst_cmap_inner: str = DEFAULT_CMAP_BURST_INNER,
         initial_burst_cmap_link: bool = True,
         initial_burst_cmap_outer: str = DEFAULT_CMAP_BURST_OUTER,
         initial_burst_color_bg: str = DEFAULT_COLOR_BG,
         initial_burst_color_bg_trnsp: bool = False,
         initial_burst_color_text: str = DEFAULT_COLOR_TEXT,
+        initial_burst_columns: int = DEFAULT_COLS_BURST,
         initial_burst_swap: bool = False,
         initial_burst_zero_fill_normalize: bool = False,
         initial_enable_cutoff: bool = True,
         initial_graph_type: TraditionalPlotType = TraditionalPlotType.NORMAL,
         initial_img_type: ImageType = ImageType.PNG,
         initial_markers: str = DEFAULT_MARKERS,
         initial_plot_style: str = DEFAULT_PLOT_STYLE,
+        initial_resolution: int = DEFAULT_RESOLUTION,
         initial_show_shadow: bool = False,
     ):
         super().__init__()
 
         if initial_plot_style not in matplotlib.style.available:
             warnings.warn(
                 f"unrecognized plot style {initial_plot_style!r}; reverting to 'default'",
@@ -573,22 +598,24 @@
         self.burst_cmap_inner.value = initial_burst_cmap_inner
         self.burst_cmap_link.value = initial_burst_cmap_link
         self.burst_cmap_outer.disabled = initial_burst_cmap_link
         self.burst_cmap_outer.value = initial_burst_cmap_outer
         self.burst_color_bg.value = initial_burst_color_bg
         self.burst_color_bg_trnsp.value = initial_burst_color_bg_trnsp
         self.burst_color_text.value = initial_burst_color_text
+        self.burst_columns.value = initial_burst_columns
         self.burst_swap.value = initial_burst_swap
         self.burst_zero_fill_normalize.value = initial_burst_zero_fill_normalize
         self.cutoff.disabled = not initial_enable_cutoff
         self.enable_cutoff.value = initial_enable_cutoff
         self.graph_type.value = initial_graph_type
         self.img_type.value = initial_img_type
         self.markers.value = initial_markers
         self.plot_style.value = initial_plot_style
+        self.resolution.value = initial_resolution
         self.show_shadow.value = initial_show_shadow
 
         def _handle_burst_cmap_link(change) -> None:
             self.burst_cmap_outer.disabled = change["new"]
 
         self.burst_cmap_link.observe(_handle_burst_cmap_link, names="value")
 
@@ -633,15 +660,15 @@
         selecting those needed by the plotter.
         """
         return widgets.VBox(
             [
                 plot_widgets.enable_cutoff,
                 plot_widgets.cutoff,
                 plot_widgets.img_type,
-                plot_widgets.scale,
+                plot_widgets.resolution,
             ]
         )
 
     @abstractmethod
     def plot(
         self,
         hs: Sequence[Tuple[str, H, Optional[H]]],
@@ -706,16 +733,16 @@
     def plot(
         self,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
         _, ax = matplotlib.pyplot.subplots(
             figsize=(
-                settings["scale"],
-                settings["scale"] / 16 * 9,
+                settings["resolution"],
+                settings["resolution"] / 16 * 9,
             )
         )
 
         plot_bar(
             ax,
             tuple((label, h) for label, h, _ in hs),
             alpha=settings["alpha"],
@@ -765,36 +792,40 @@
                         ),
                         widgets.VBox(
                             [
                                 plot_widgets.alpha,
                                 plot_widgets.burst_color_text,
                                 plot_widgets.burst_color_bg,
                                 plot_widgets.burst_color_bg_trnsp,
+                                plot_widgets.burst_columns,
                             ]
                         ),
                     ]
                 ),
             ]
         )
 
     @beartype
     def plot(
         self,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
-        cols = 3
+        cols = settings["burst_columns"]
+        assert cols > 0
         logical_rows = len(hs) // cols + (len(hs) % cols != 0)
         # Height of row gaps in relation to height of figs
         gap_size_ratio = Fraction(1, 5)
         total_gaps = max(0, logical_rows - 1)
         figsize = (
-            settings["scale"],
+            settings["resolution"],
             float(
-                settings["scale"] * (logical_rows + total_gaps * gap_size_ratio) / cols
+                settings["resolution"]
+                * (logical_rows + total_gaps * gap_size_ratio)
+                / cols
             ),
         )
         matplotlib.pyplot.figure(facecolor=settings["burst_color_bg"], figsize=figsize)
         actual_rows_per_fig = gap_size_ratio.denominator
         actual_rows_per_gap = gap_size_ratio.numerator
         total_actual_rows = (
             logical_rows * actual_rows_per_fig + total_gaps * actual_rows_per_gap
@@ -872,17 +903,17 @@
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
         total_outcomes = sum(
             1 for _ in chain.from_iterable(h.outcomes() for _, h, _ in hs)
         )
         total_height = total_outcomes + 1  # one extra to accommodate the axis
-        inches_per_height_unit = settings["scale"] / 64
+        inches_per_height_unit = settings["resolution"] / 64
         figsize = (
-            settings["scale"],
+            settings["resolution"],
             total_height * inches_per_height_unit,
         )
         matplotlib.pyplot.figure(figsize=figsize)
         barh_kw: Dict[str, Any] = dict(alpha=settings["alpha"])
 
         if settings["show_shadow"]:
             barh_kw.update(
@@ -979,16 +1010,16 @@
     def plot(
         self,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
         _, ax = matplotlib.pyplot.subplots(
             figsize=(
-                settings["scale"],
-                settings["scale"] / 16 * 9,
+                settings["resolution"],
+                settings["resolution"] / 16 * 9,
             )
         )
 
         plot_line(
             ax,
             tuple((label, h) for label, h, _ in hs),
             alpha=settings["alpha"],
@@ -1019,16 +1050,16 @@
     def plot(
         self,
         hs: Sequence[Tuple[str, H, Optional[H]]],
         settings: SettingsDict,
     ) -> None:
         _, ax = matplotlib.pyplot.subplots(
             figsize=(
-                settings["scale"],
-                settings["scale"] / 16 * 9,
+                settings["resolution"],
+                settings["resolution"] / 16 * 9,
             )
         )
 
         plot_scatter(
             ax,
             tuple((label, h) for label, h, _ in hs),
             alpha=settings["alpha"],
@@ -1050,17 +1081,28 @@
         future versions.
 
     A controller for coordinating the display of a histogram data set and selection of
     one or more plotters as well as triggering updates in response to either control or
     data changes. All parameters for the
     [initializer][anydyce.viz.HPlotterChooser.__init__] are optional.
 
-    *histogram_specs* is the histogram data set which defaults to an empty tuple. The
-    histogram data set can also be replaced vi the
-    [``update_hs``][anydyce.viz.HPlotterChooser.update_hs] method.
+    *histogram_specs* is the histogram data set which defaults to an empty tuple. If
+    provided, each item therein can be a ``#!python dyce.H`` object, a 2-tuple, or a
+    3-tuple. 2-tuples are in the format ``#!python (str, H)``, where ``#!python str`` is
+    a name or description that will be used to identify the accompanying ``#!python H``
+    object where it appears in the visualization. 3-tuples are in the format ``#!python
+    (str, H, H)``. The second ``#!python H`` object is used for the interior ring in
+    “burst” break-out graphs, but otherwise ignored. If an item is ``#!python None``, it
+    is roughly synonymous with ``#!python ("", H({}), None)``, with the exception that
+    it does not advance the automatic naming counter. This can be useful as “blank”
+    filler to achieve a desired layout (e.g., where one wants to compare across burst
+    graphs that don't neatly fit into a particular row size).
+
+    The histogram data set can also be replaced via
+    [``update_hs``][anydyce.viz.HPlotterChooser.update_hs].
 
     Plotter controls (including the selection tabs) are contained within an accordion
     interface. If *controls_expanded* is ``#!python True``, the accordion is initially
     expanded for the user. If it is ``#!python False``, it is initially collapsed.
 
     *plot_widgets* allows object creators to customize the available control widgets,
     including their initial values. It defaults to ``#!python None`` which results in a
@@ -1075,15 +1117,17 @@
     provided by the *plotters_or_factories* parameter.
     """
 
     @beartype
     def __init__(
         self,
         histogram_specs: Iterable[
-            Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
+            Optional[
+                Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
+            ]
         ] = (),
         *,
         controls_expanded: bool = False,
         plot_widgets: Optional[PlotWidgets] = None,
         plotters_or_factories: Iterable[Union[HPlotter, HPlotterFactoryT]] = (
             BurstHPlotter,
             LineHPlotter,
@@ -1226,23 +1270,23 @@
             matplotlib.pyplot.clf()
             matplotlib.pyplot.close()
 
     @beartype
     def update_hs(
         self,
         histogram_specs: Iterable[
-            Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
+            Optional[
+                Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
+            ]
         ],
     ) -> None:
         r"""
-        Triggers an update to the histogram data. *histogram_specs* is an iterable of either
-        a single [``HLikeT``][anydyce.viz.HLikeT] object, a two-tuple of a name and a
-        primary ``HLikeT`` object, or a three-tuple of a name, a primary ``HLikeT``
-        object, and an optional secondary ``HLikeT`` object (``#!python None`` if
-        omitted).
+        Triggers an update to the histogram data. See
+        [``HPlotterChooser``][anydyce.viz.HPlotterChooser] for a more detailed
+        explanation of *histogram_specs*.
         """
         self._hs = _histogram_specs_to_h_tuples(histogram_specs, cutoff=None)
         self._csv_download_link = _csv_download_link(self._hs)
 
         self._plot_widgets.burst_swap.disabled = all(
             h_outer is None or h_inner == h_outer for _, h_inner, h_outer in self._hs
         )
@@ -1462,15 +1506,16 @@
 
     return H(_cull())
 
 
 @experimental
 @beartype
 def values_xy_for_graph_type(
-    h: H, graph_type: TraditionalPlotType
+    h: H,
+    graph_type: TraditionalPlotType,
 ) -> Tuple[Tuple[RealLike, ...], Tuple[float, ...]]:
     outcomes, probabilities = h.distribution_xy() if h else ((), ())
 
     if graph_type is TraditionalPlotType.AT_LEAST:
         probabilities = tuple(accumulate(probabilities, __sub__, initial=1.0))[:-1]
     elif graph_type is TraditionalPlotType.AT_MOST:
         probabilities = tuple(accumulate(probabilities, __add__, initial=0.0))[1:]
@@ -1787,52 +1832,49 @@
     return fig, ax
 
 
 @experimental
 @beartype
 def jupyter_visualize(
     histogram_specs: Iterable[
-        Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
+        Optional[
+            Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
+        ]
     ],
     *,
     controls_expanded: bool = False,
     initial_alpha: float = DEFAULT_ALPHA,
     initial_burst_cmap_inner: str = DEFAULT_CMAP_BURST_INNER,
     initial_burst_cmap_link: bool = True,
     initial_burst_cmap_outer: str = DEFAULT_CMAP_BURST_OUTER,
     initial_burst_color_bg: str = DEFAULT_COLOR_BG,
     initial_burst_color_bg_trnsp: bool = False,
     initial_burst_color_text: str = DEFAULT_COLOR_TEXT,
+    initial_burst_columns: int = DEFAULT_COLS_BURST,
     initial_burst_swap: bool = False,
     initial_burst_zero_fill_normalize: bool = False,
     initial_enable_cutoff: bool = True,
     initial_graph_type: TraditionalPlotType = TraditionalPlotType.NORMAL,
     initial_img_type: ImageType = ImageType.PNG,
     initial_markers: str = DEFAULT_MARKERS,
     initial_plot_style: str = DEFAULT_PLOT_STYLE,
+    initial_resolution: int = DEFAULT_RESOLUTION,
     initial_show_shadow: bool = False,
     selected_name: Optional[str] = None,
 ):
     r"""
     !!! warning "Experimental"
 
         This function should be considered experimental and may change or disappear in
         future versions.
 
     Takes a list of one or more *histogram_specs* and produces an interactive
     visualization reminiscent of [AnyDice](https://anydice.com/), but with some extra
     goodies.
 
-    Each item in *histogram_specs* can be a ``#!python dyce.H`` object, a 2-tuple, or a
-    3-tuple. 2-tuples are in the format ``#!python (str, H)``, where ``#!python str`` is
-    a name or description that will be used to identify the accompanying ``#!python H``
-    object where it appears in the visualization. 3-tuples are in the format ``#!python
-    (str, H, H)``. The second ``#!python H`` object is used for the interior ring in
-    “burst” break-out graphs, but otherwise ignored.
-
     The “Powered by the _Apocalypse_ (PbtA)” example in the introduction notebook should
     give an idea of the effect. (See [Interactive quick
     start](index.md#interactive-quick-start).)
 
     Parameters have the same meanings as with
     [``HPlotterChooser``][anydyce.viz.HPlotterChooser] and
     [``PlotWidgets``][anydyce.viz.PlotWidgets].
@@ -1844,21 +1886,23 @@
             initial_alpha=initial_alpha,
             initial_burst_cmap_inner=initial_burst_cmap_inner,
             initial_burst_cmap_link=initial_burst_cmap_link,
             initial_burst_cmap_outer=initial_burst_cmap_outer,
             initial_burst_color_bg=initial_burst_color_bg,
             initial_burst_color_bg_trnsp=initial_burst_color_bg_trnsp,
             initial_burst_color_text=initial_burst_color_text,
+            initial_burst_columns=initial_burst_columns,
             initial_burst_swap=initial_burst_swap,
             initial_burst_zero_fill_normalize=initial_burst_zero_fill_normalize,
             initial_enable_cutoff=initial_enable_cutoff,
             initial_graph_type=initial_graph_type,
             initial_img_type=initial_img_type,
             initial_markers=initial_markers,
             initial_plot_style=initial_plot_style,
+            initial_resolution=initial_resolution,
             initial_show_shadow=initial_show_shadow,
         ),
         selected_name=selected_name,
     )
 
     plotter_chooser.interact()
 
@@ -1886,32 +1930,40 @@
 
     return f'<a download="{csv_name}.csv" href="data:text/csv;base64,{payload}" target="_blank">Download raw data as CSV</a>'
 
 
 @beartype
 def _histogram_specs_to_h_tuples(
     histogram_specs: Iterable[
-        Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
+        Optional[
+            Union[HLikeT, Tuple[str, HLikeT], Tuple[str, HLikeT, Optional[HLikeT]]]
+        ]
     ],
     cutoff: Optional[float] = None,
 ) -> Tuple[Tuple[str, H, Optional[H]], ...]:
     h_specs = []
 
     if cutoff is None:
         cutoff_frac = Fraction(0, 1)
     else:
         cutoff_frac = Fraction(cutoff).limit_denominator(_CUTOFF_BASE**_CUTOFF_EXP)
 
     label: str
     first_h_like: HLikeT
     second_h_like: Optional[HLikeT]
+    num_blanks = 0
 
     for i, thing in enumerate(histogram_specs):
-        if isinstance(thing, (H, HableT)):
-            label = f"Histogram {i + 1}"
+        if thing is None:
+            label = ""
+            first_h_like = H({})
+            second_h_like = None
+            num_blanks += 1
+        elif isinstance(thing, (H, HableT)):
+            label = f"Histogram {i - num_blanks + 1}"
             first_h_like = thing
             second_h_like = None
         else:
             label, first_h_like = thing[:2]
 
             if len(thing) >= 3:
                 # TODO(posita): See <https://github.com/python/mypy/issues/1178>
```

## Comparing `anydyce-0.4.3.dist-info/LICENSE` & `anydyce-0.4.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anydyce-0.4.3.dist-info/METADATA` & `anydyce-0.4.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydyce
-Version: 0.4.3
+Version: 0.4.4
 Summary: Visualization tools for dyce
 Home-page: https://posita.github.io/anydyce/
 Author: Matt Bogosian
 Author-email: matt@bogosian.net
 License: MIT License
 Project-URL: Source Repository, https://github.com/posita/anydyce/
 Classifier: Topic :: Education
@@ -51,19 +51,19 @@
 
 *Copyright and other protections apply.
 Please see the accompanying ``LICENSE`` file for rights and restrictions governing use of this software.
 All rights not expressly waived or licensed are reserved.
 If that file is missing or appears to be modified from its original, then please contact the author before viewing or using this software in any capacity.*
 
 [![Tests](https://github.com/posita/anydyce/actions/workflows/on-push.yaml/badge.svg)](https://github.com/posita/anydyce/actions/workflows/on-push.yaml)
-[![Version](https://img.shields.io/pypi/v/anydyce/0.4.3.svg)](https://pypi.org/project/anydyce/0.4.3/)
-[![Development Stage](https://img.shields.io/pypi/status/anydyce/0.4.3.svg)](https://pypi.org/project/anydyce/0.4.3/)
-[![License](https://img.shields.io/pypi/l/anydyce/0.4.3.svg)](http://opensource.org/licenses/MIT)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/anydyce/0.4.3.svg)](https://pypi.org/project/anydyce/0.4.3/)
-[![Supported Python Implementations](https://img.shields.io/pypi/implementation/anydyce/0.4.3.svg)](https://pypi.org/project/anydyce/0.4.3/)
+[![Version](https://img.shields.io/pypi/v/anydyce/0.4.4.svg)](https://pypi.org/project/anydyce/0.4.4/)
+[![Development Stage](https://img.shields.io/pypi/status/anydyce/0.4.4.svg)](https://pypi.org/project/anydyce/0.4.4/)
+[![License](https://img.shields.io/pypi/l/anydyce/0.4.4.svg)](http://opensource.org/licenses/MIT)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/anydyce/0.4.4.svg)](https://pypi.org/project/anydyce/0.4.4/)
+[![Supported Python Implementations](https://img.shields.io/pypi/implementation/anydyce/0.4.4.svg)](https://pypi.org/project/anydyce/0.4.4/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![``dyce``-powered!](https://raw.githubusercontent.com/posita/dyce/latest/docs/dyce-powered.svg)](https://posita.github.io/dyce/)
 [![``numerary``-encumbered](https://raw.githubusercontent.com/posita/numerary/latest/docs/numerary-encumbered.svg)](https://posita.github.io/numerary/)
 [![Bear-ified™](https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg)](https://beartype.rtfd.io/)
 
 # ``anydyce`` – visualization tools for [``dyce``](https://posita.github.io/dyce/)
 
@@ -112,15 +112,15 @@
     Notebooks can also be downloaded and shared as ``.ipynb`` files.
 
 ### Interactive quick start
 
 Probably the _easiest_ way to start tinkering with ``anydyce`` is with [JupyterLite](https://jupyterlite.readthedocs.io/):
 [![Try dyce](https://jupyterlite.readthedocs.io/en/latest/_static/badge.svg)](https://posita.github.io/anydyce/0.4/jupyter/lab/?path=anydyce_intro.ipynb)
 
-The [``quickstart-local.sh`` script](https://github.com/posita/anydyce/blob/v0.4.3/quickstart-local.sh) will create a local [virtual environment](https://docs.python.org/3/library/venv.html) to bootstrap a local Jupyter server with ``anydyce`` installed and open a web browser to the [introduction notebook](https://github.com/posita/anydyce/blob/v0.4.3/docs/notebooks/anydyce_intro-ipynb).
+The [``quickstart-local.sh`` script](https://github.com/posita/anydyce/blob/v0.4.4/quickstart-local.sh) will create a local [virtual environment](https://docs.python.org/3/library/venv.html) to bootstrap a local Jupyter server with ``anydyce`` installed and open a web browser to the [introduction notebook](https://github.com/posita/anydyce/blob/v0.4.4/docs/notebooks/anydyce_intro-ipynb).
 
 [Binder](https://mybinder.org/) is another great resource that you can use to share notebooks from your Git repositories (including [Gists](https://gist.github.com/)):
 [![Try dyce](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/posita/anydyce/HEAD?labpath=docs%2Fnotebooks%2Fanydyce_intro.ipynb)
 
 !!! danger "JupyterLite and Binder may not save your work!"
 
     JupyterLite attempts to make use of your browser’s local storage for saving notebook changes.
@@ -160,20 +160,20 @@
 >>> plot_burst(ax, 2@H(6))
 >>> matplotlib.pyplot.show()  # doctest: +SKIP
 
 ```
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_1_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: Basic plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_1_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_1_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_1_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: Basic plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_1_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_1_dark.png#gh-dark-mode-only"></span>
 </picture>
 
 <details>
-<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_1.py"><code>plot_burst_1.py</code></a></summary>
+<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_1.py"><code>plot_burst_1.py</code></a></summary>
 
 ``` python
 --8<-- "docs/assets/plot_burst_1.py"
 ```
 </details>
 
 The outer ring can also be used to compare two histograms directly.
@@ -193,20 +193,20 @@
 ... )
 >>> matplotlib.pyplot.show()  # doctest: +SKIP
 
 ```
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_2_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: 2d6 vs. 4dF plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_2_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_2_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_2_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: 2d6 vs. 4dF plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_2_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_2_dark.png#gh-dark-mode-only"></span>
 </picture>
 
 <details>
-<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_2.py"><code>plot_burst_2.py</code></a></summary>
+<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_2.py"><code>plot_burst_2.py</code></a></summary>
 
 ``` python
 --8<-- "docs/assets/plot_burst_2.py"
 ```
 </details>
 
 Labels can even be overridden for interesting, at-a-glance displays.
@@ -232,20 +232,20 @@
 ... }), inner_cmap="RdYlBu_r", outer_formatter=d20formatter)
 >>> matplotlib.pyplot.show()  # doctest: +SKIP
 
 ```
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_3_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: Advanced plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_3_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_3_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_3_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: Advanced plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_3_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_3_dark.png#gh-dark-mode-only"></span>
 </picture>
 
 <details>
-<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_3.py"><code>plot_burst_3.py</code></a></summary>
+<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.4/docs/assets/plot_burst_3.py"><code>plot_burst_3.py</code></a></summary>
 
 ``` python
 --8<-- "docs/assets/plot_burst_3.py"
 ```
 </details>
 
 ### Requirements
```

