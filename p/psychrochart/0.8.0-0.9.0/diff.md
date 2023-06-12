# Comparing `tmp/psychrochart-0.8.0.tar.gz` & `tmp/psychrochart-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychrochart-0.8.0.tar", max compression
+gzip compressed data, was "psychrochart-0.9.0.tar", max compression
```

## Comparing `psychrochart-0.8.0.tar` & `psychrochart-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     9831 2023-06-11 10:04:18.635505 psychrochart-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-06-11 10:04:18.635505 psychrochart-0.8.0/LICENSE
--rw-r--r--   0        0        0     7077 2023-06-11 10:04:18.635505 psychrochart-0.8.0/README.md
--rw-r--r--   0        0        0      711 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/__init__.py
--rw-r--r--   0        0        0      336 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/__main__.py
--rw-r--r--   0        0        0    13944 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart.py
--rw-r--r--   0        0        0     2231 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_entities.py
--rw-r--r--   0        0        0     2157 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/ashrae_chart_style.json
--rw-r--r--   0        0        0     2380 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
--rw-r--r--   0        0        0     3097 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/default_chart_config.json
--rw-r--r--   0        0        0      585 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/default_comfort_zones.json
--rw-r--r--   0        0        0     2436 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/interior_chart_style.json
--rw-r--r--   0        0        0     2490 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chart_styles/minimal_chart_style.json
--rw-r--r--   0        0        0    15847 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chartdata.py
--rw-r--r--   0        0        0     2296 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/chartzones.py
--rw-r--r--   0        0        0        0 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/__init__.py
--rw-r--r--   0        0        0     3350 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/annots.py
--rw-r--r--   0        0        0     1246 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/base.py
--rw-r--r--   0        0        0     8628 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/config.py
--rw-r--r--   0        0        0     3604 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/curves.py
--rw-r--r--   0        0        0     5844 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/parsers.py
--rw-r--r--   0        0        0     1909 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/styles.py
--rw-r--r--   0        0        0     1924 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/models/validators.py
--rw-r--r--   0        0        0    15951 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/plot_logic.py
--rw-r--r--   0        0        0     7978 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/process_logic.py
--rw-r--r--   0        0        0     3977 2023-06-11 10:04:18.651506 psychrochart-0.8.0/psychrochart/util.py
--rw-r--r--   0        0        0     2222 2023-06-11 10:04:18.651506 psychrochart-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8406 1970-01-01 00:00:00.000000 psychrochart-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11085 2023-06-12 15:33:00.015983 psychrochart-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-06-12 15:33:00.015983 psychrochart-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7077 2023-06-12 15:33:00.015983 psychrochart-0.9.0/README.md
+-rw-r--r--   0        0        0      739 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/__main__.py
+-rw-r--r--   0        0        0    15270 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart.py
+-rw-r--r--   0        0        0     2231 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_entities.py
+-rw-r--r--   0        0        0     2157 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/ashrae_chart_style.json
+-rw-r--r--   0        0        0     2380 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
+-rw-r--r--   0        0        0     3097 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/default_chart_config.json
+-rw-r--r--   0        0        0      585 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/default_comfort_zones.json
+-rw-r--r--   0        0        0     2436 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/interior_chart_style.json
+-rw-r--r--   0        0        0     2490 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chart_styles/minimal_chart_style.json
+-rw-r--r--   0        0        0    15847 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chartdata.py
+-rw-r--r--   0        0        0    14504 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/chartzones.py
+-rw-r--r--   0        0        0        0 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/__init__.py
+-rw-r--r--   0        0        0     3350 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/annots.py
+-rw-r--r--   0        0        0     1246 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/base.py
+-rw-r--r--   0        0        0     8656 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/config.py
+-rw-r--r--   0        0        0     3945 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/curves.py
+-rw-r--r--   0        0        0     5844 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/parsers.py
+-rw-r--r--   0        0        0     1909 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/styles.py
+-rw-r--r--   0        0        0     1924 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/models/validators.py
+-rw-r--r--   0        0        0    15798 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/plot_logic.py
+-rw-r--r--   0        0        0     8135 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/process_logic.py
+-rw-r--r--   0        0        0     4631 2023-06-12 15:33:00.031983 psychrochart-0.9.0/psychrochart/util.py
+-rw-r--r--   0        0        0     2222 2023-06-12 15:33:00.031983 psychrochart-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8406 1970-01-01 00:00:00.000000 psychrochart-0.9.0/PKG-INFO
```

### Comparing `psychrochart-0.8.0/CHANGELOG.md` & `psychrochart-0.9.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.0] - ✨ More kinds of chart zones + CSS for SVG styling - 2023-06-12
+
+Define new enclosed areas in chart between constant RH lines and constant volume or enthalpy values,
+and enable full potencial for SVG customization by including CSS and/or `<defs>` inside it.
+
+##### Changes
+
+- ✨ Add new kind of overlay **zones 'enthalpy-rh' and 'volume-rh'**, to define chart areas delimited between 2 constant enthalpy or volume lines, and 2 constant humidity lines
+- 🎨 Add `chart.remove_zones()` method, like the existent `.remove_legend()` and `.remove_annotations()`, to clear matplotlib current Axes from each kind of annotated objects
+- 🐛 Fix artists registry not mirroring objects in plot, by setting a new one each time `chart.plot()` is invoked
+- ♻️ Set gid for 'chart_legend_background' item if frameon is enabled
+- ✨ Pass **optional CSS and SVG <defs>** to `chart.make_svg()`, to include extra-styling inside the produced SVG 🌈
+- ✨ Add method `chart.plot_over_saturated_zone()` to create a filled patch in the over-saturated zone of the psychrochart, to colorize that area
+- 🦄 tests: Add dynamic effects and CSS rules to splash chart for a show-off of SVG styling capabilities
+- 🚀 env: Bump version and update CHANGELOG
+
 ## [0.8.0] - ✨ Lazy generation of chart data, 'Artist' registry, and better SVG export - 2023-06-11
 
 Now all chart-data parameters, including the overlayed zones, are included in the `ChartConfig`,
 and generation of curves only happens when chart is plotted (or saved to disk).
 
 Any change in the chart configuration will trigger a data-regen for all items before plotting.
```

### Comparing `psychrochart-0.8.0/LICENSE` & `psychrochart-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/README.md` & `psychrochart-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/__init__.py` & `psychrochart-0.9.0/psychrochart/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """A library to make psychrometric charts and overlay information in them."""
 from psychrochart.chart import PsychroChart
 from psychrochart.models.annots import ChartAnnots
-from psychrochart.models.config import ChartConfig, ChartZones
+from psychrochart.models.config import ChartConfig, ChartZone, ChartZones
 from psychrochart.models.curves import PsychroCurve, PsychroCurves
 from psychrochart.models.parsers import load_config, load_zones
 from psychrochart.models.styles import (
     CurveStyle,
     LabelStyle,
     TickStyle,
     ZoneStyle,
 )
 
 __all__ = [
     "ChartAnnots",
     "ChartConfig",
     "ChartZones",
+    "ChartZone",
     "load_config",
     "load_zones",
     "PsychroChart",
     "PsychroCurve",
     "PsychroCurves",
     "CurveStyle",
     "LabelStyle",
```

### Comparing `psychrochart-0.8.0/psychrochart/chart.py` & `psychrochart-0.9.0/psychrochart/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,18 @@
     reg_artist,
 )
 from psychrochart.chartdata import (
     gen_points_in_constant_relative_humidity,
     make_constant_dry_bulb_v_line,
     make_saturation_line,
 )
+from psychrochart.chartzones import make_over_saturated_zone
 from psychrochart.models.annots import ChartAnnots
 from psychrochart.models.config import ChartConfig, ChartZones
-from psychrochart.models.curves import PsychroChartModel
+from psychrochart.models.curves import PsychroChartModel, PsychroCurve
 from psychrochart.models.parsers import (
     ConvexGroupTuple,
     load_extra_annots,
     load_points_dbt_rh,
     obj_loader,
 )
 from psychrochart.models.styles import CurveStyle
@@ -37,15 +38,15 @@
     plot_chart,
     plot_curve,
 )
 from psychrochart.process_logic import (
     get_pressure_pa,
     update_psychrochart_data,
 )
-from psychrochart.util import mod_color
+from psychrochart.util import add_styling_to_svg, mod_color
 
 
 def _select_fig_canvas(
     path_dest: Any, canvas_cls: Type[FigureCanvasBase] | None = None
 ) -> Type[FigureCanvasBase]:
     if (
         canvas_cls is None
@@ -304,44 +305,65 @@
                 make_item_gid(
                     "label-vline", family_label="constant-dbt", name=label
                 ),
                 add_label_to_curve(curve, self.axes, label, **label_params),
                 self._artists.annotations,
             )
 
+    def plot_over_saturated_zone(
+        self, color_fill: str | list[float] = "#0C92F6FF"
+    ) -> PsychroCurve | None:
+        """Add a colored zone in chart to fill the over-saturated space."""
+        # ensure chart is plotted
+        current_ax = self.axes
+        if (
+            curve_sat_zone := make_over_saturated_zone(
+                self.saturation,
+                dbt_min=self.config.dbt_min,
+                dbt_max=self.config.dbt_max,
+                w_min=self.config.w_min,
+                w_max=self.config.w_max,
+                color_fill=color_fill,
+            )
+        ) is not None:
+            plot_curve(curve_sat_zone, current_ax)
+            self._artists.zones.update()
+        return curve_sat_zone
+
     def plot_legend(
         self,
         loc: str = "upper left",
         markerscale: float = 0.9,
         frameon: bool = True,
         fancybox: bool = True,
         edgecolor: str | Iterable = "darkgrey",
         fontsize: float = 15.0,
         labelspacing: float = 1.5,
         **params,
     ) -> None:
         """Append a legend to the psychrochart plot."""
-        reg_artist(
-            "chart_legend",
-            self.axes.legend(
-                loc=loc,
-                markerscale=markerscale,
-                frameon=frameon,
-                edgecolor=edgecolor,
-                fontsize=fontsize,
-                fancybox=fancybox,
-                labelspacing=labelspacing,
-                **params,
-            ),
-            self._artists.layout,
+        legend = self.axes.legend(
+            loc=loc,
+            markerscale=markerscale,
+            frameon=frameon,
+            edgecolor=edgecolor,
+            fontsize=fontsize,
+            fancybox=fancybox,
+            labelspacing=labelspacing,
+            **params,
         )
+        if frameon:
+            legend.get_frame().set_gid("chart_legend_background")
+        reg_artist("chart_legend", legend, self._artists.layout)
 
     def plot(self, ax: Axes | None = None) -> Axes:
         """Plot the psychrochart and return the matplotlib Axes instance."""
         self.process_chart()
+        # instantiate a new artist registry for the new plot
+        self._artists = ChartRegistry()
         if ax is not None:
             self._fig = ax.get_figure()
         else:
             self._fig = figure.Figure(
                 figsize=self.config.figure.figsize,
                 dpi=self.config.figure.dpi,
                 frameon=False,
@@ -353,14 +375,20 @@
         self._axes = ax
         self._artists.layout.update(
             apply_axis_styling(self.config, self._axes)
         )
         plot_chart(self, self._axes, self._artists)
         return self._axes
 
+    def remove_zones(self) -> None:
+        """Remove the zones in the chart to reuse it."""
+        for patch in self._artists.zones.values():
+            patch.remove()
+        self._artists.zones = {}
+
     def remove_annotations(self) -> None:
         """Remove the annotations made in the chart to reuse it."""
         for line in self._artists.annotations.values():
             line.remove()
         self._artists.annotations = {}
 
     def remove_legend(self) -> None:
@@ -384,20 +412,25 @@
         if not self.rendered or self.config.has_changed:
             self.plot()
         assert self._fig is not None
         canvas_use = _select_fig_canvas(path_dest, canvas_cls)
         canvas_use(self._fig).print_figure(path_dest, **params)
         gc.collect()
 
-    def make_svg(self, **params) -> str:
+    def make_svg(
+        self,
+        css_styles: str | Path | None = None,
+        svg_definitions: str | None = None,
+        **params,
+    ) -> str:
         """Generate chart as SVG and return as text."""
         svg_io = StringIO()
         self.save(svg_io, canvas_cls=FigureCanvasSVG, **params)
         svg_io.seek(0)
-        return svg_io.read()
+        return add_styling_to_svg(svg_io.read(), css_styles, svg_definitions)
 
     def close_fig(self) -> None:
         """Close the figure plot."""
         assert self._axes is not None
         assert self._fig is not None
         self.remove_annotations()
         self.remove_legend()
```

### Comparing `psychrochart-0.8.0/psychrochart/chart_entities.py` & `psychrochart-0.9.0/psychrochart/chart_entities.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/chart_styles/ashrae_chart_style.json` & `psychrochart-0.9.0/psychrochart/chart_styles/ashrae_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/chart_styles/ashrae_ip_chart_style.json` & `psychrochart-0.9.0/psychrochart/chart_styles/ashrae_ip_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/chart_styles/default_chart_config.json` & `psychrochart-0.9.0/psychrochart/chart_styles/default_chart_config.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/chart_styles/default_comfort_zones.json` & `psychrochart-0.9.0/psychrochart/chart_styles/default_comfort_zones.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/chart_styles/interior_chart_style.json` & `psychrochart-0.9.0/psychrochart/chart_styles/interior_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/chart_styles/minimal_chart_style.json` & `psychrochart-0.9.0/psychrochart/chart_styles/minimal_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/chartdata.py` & `psychrochart-0.9.0/psychrochart/chartdata.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/models/annots.py` & `psychrochart-0.9.0/psychrochart/models/annots.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/models/base.py` & `psychrochart-0.9.0/psychrochart/models/base.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/models/config.py` & `psychrochart-0.9.0/psychrochart/models/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 _DEFAULT_STYLE_DRY_TEMP = CurveStyle(
     color=[0.855, 0.145, 0.114], linewidth=0.75, linestyle=":"
 )
 _DEFAULT_STYLE_HUMID = CurveStyle(
     color=[0.0, 0.125, 0.376], linewidth=0.75, linestyle=":"
 )
 
-ZoneKind = Literal["dbt-rh", "xy-points"]
+ZoneKind = Literal["dbt-rh", "xy-points", "enthalpy-rh", "volume-rh"]
 
 
 class ChartFigure(BaseConfig):
     """Psychrochart settings for matplotlib Figure."""
 
     figsize: tuple[float, float] = Field(default=(16, 9))
     dpi: int = Field(default=150)
```

### Comparing `psychrochart-0.8.0/psychrochart/models/curves.py` & `psychrochart-0.9.0/psychrochart/models/curves.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,25 @@
             "PsychroZone"
             if isinstance(self.style, ZoneStyle)
             else "PsychroCurve"
         )
         extra = f" (label: {self.label})" if self.label else ""
         return f"<{name} {len(self.x_data)} values{extra}>"
 
+    def outside_limits(
+        self, xmin: float, xmax: float, ymin: float, ymax: float
+    ) -> bool:
+        """Test if curve is invisible (outside box)."""
+        return (
+            max(self.y_data) < ymin
+            or max(self.x_data) < xmin
+            or min(self.y_data) > ymax
+            or min(self.x_data) > xmax
+        )
+
 
 class PsychroCurves(BaseModel):
     """Pydantic model to store a list of psychrometric curves for plotting."""
 
     curves: list[PsychroCurve] = Field(min_items=1)
     family_label: str | None = None
```

### Comparing `psychrochart-0.8.0/psychrochart/models/parsers.py` & `psychrochart-0.9.0/psychrochart/models/parsers.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/models/styles.py` & `psychrochart-0.9.0/psychrochart/models/styles.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/models/validators.py` & `psychrochart-0.9.0/psychrochart/models/validators.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.8.0/psychrochart/plot_logic.py` & `psychrochart-0.9.0/psychrochart/plot_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,27 +115,20 @@
 def plot_curve(
     curve: PsychroCurve, ax: Axes, label_prefix: str | None = None
 ) -> dict[str, Artist]:
     """Plot the curve, if it's between chart limits."""
     artists: dict[str, Artist] = {}
     xmin, xmax = ax.get_xlim()
     ymin, ymax = ax.get_ylim()
-    if (
-        curve.x_data is None
-        or curve.y_data is None
-        or max(curve.y_data) < ymin
-        or max(curve.x_data) < xmin
-        or min(curve.y_data) > ymax
-        or min(curve.x_data) > xmax
-    ):
+    if curve.outside_limits(xmin, xmax, ymin, ymax):
         logging.info(
-            "%s (label:%s) not between limits ([%.2g, %.2g, %.2g, %.2g]) "
+            "%s (name:%s) not between limits ([%.2g, %.2g, %.2g, %.2g]) "
             "-> x:%s, y:%s",
             curve.type_curve,
-            curve.label or "unnamed",
+            curve.label or str(curve.internal_value),
             xmin,
             xmax,
             ymin,
             ymax,
             curve.x_data,
             curve.y_data,
         )
```

### Comparing `psychrochart-0.8.0/psychrochart/process_logic.py` & `psychrochart-0.9.0/psychrochart/process_logic.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     set_unit_system(unit_system_si)
     if limits.pressure_kpa is not None:
         return limits.pressure_kpa * 1000.0  # to Pa
     else:
         return GetStandardAtmPressure(limits.altitude_m)
 
 
-def _generate_chart_curves(config: ChartConfig, chart: PsychroChartModel):
+def _gen_interior_lines(config: ChartConfig, chart: PsychroChartModel) -> None:
     # check chart limits are not fully above the saturation curve!
     assert (chart.saturation.y_data > config.w_min).any()
     # check if sat curve cuts x-axis with T > config.dbt_min
     dbt_min_seen: float | None = None
     if chart.saturation.y_data[0] < config.w_min:
         temp_sat_interpolator = interp1d(
             chart.saturation.y_data,
@@ -178,14 +178,34 @@
             label_loc=config.chart_params.constant_wet_temp_labels_loc,
             family_label=config.chart_params.constant_wet_temp_label,
         )
     else:
         chart.constant_wbt_data = None
 
 
+def _gen_chart_zones(config: ChartConfig, chart: PsychroChartModel) -> None:
+    # regen all zones
+    if config.chart_params.with_zones and not config.chart_params.zones:
+        # add default zones
+        config.chart_params.zones = DEFAULT_ZONES.zones
+    zone_curves = [
+        make_zone_curve(
+            zone,
+            pressure=chart.pressure,
+            step_temp=config.limits.step_temp,
+            dbt_min=config.dbt_min,
+            dbt_max=config.dbt_max,
+            w_min=config.w_min,
+            w_max=config.w_max,
+        )
+        for zone in config.chart_params.zones
+    ]
+    chart.zones = [zc for zc in zone_curves if zc is not None]
+
+
 def update_psychrochart_data(
     current_chart: PsychroChartModel, config: ChartConfig
 ) -> None:
     """Update the PsychroChart data with config changes."""
     if config.limits.has_changed:
         current_chart.altitude_m = config.limits.altitude_m
         current_chart.pressure = get_pressure_pa(
@@ -196,25 +216,11 @@
     current_chart.saturation = make_saturation_line(
         config.dbt_min,
         config.dbt_max,
         config.limits.step_temp,
         current_chart.pressure,
         style=config.saturation,
     )
-    _generate_chart_curves(config, current_chart)
+    _gen_interior_lines(config, current_chart)
     # regen all zones
-    if config.chart_params.with_zones and not config.chart_params.zones:
-        # add default zones
-        config.chart_params.zones = DEFAULT_ZONES.zones
-    zone_curves = [
-        make_zone_curve(
-            zone,
-            pressure=current_chart.pressure,
-            step_temp=config.limits.step_temp,
-            # dbt_min=config.dbt_min,
-            # dbt_max=config.dbt_max,
-            # w_min=config.w_min,
-        )
-        for zone in config.chart_params.zones
-    ]
-    current_chart.zones = [zc for zc in zone_curves if zc is not None]
+    _gen_chart_zones(config, current_chart)
     config.commit_changes()
```

### Comparing `psychrochart-0.8.0/psychrochart/util.py` & `psychrochart-0.9.0/psychrochart/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+from pathlib import Path
 from typing import Callable, Sequence
 
 import numpy as np
 
 NUM_ITERS_MAX = 100
 TESTING_MODE = os.getenv("PYTEST_CURRENT_TEST") is not None
 
@@ -107,7 +108,28 @@
     if abs(modification) < 0.999:  # is alpha level
         color = list(color[:3]) + [modification]
     else:
         color = [
             max(0.0, min(1.0, c * (1 + modification / 100))) for c in color
         ]
     return color
+
+
+def add_styling_to_svg(
+    original: str,
+    css_styles: str | Path | None = None,
+    svg_definitions: str | None = None,
+) -> str:
+    """Insert CSS styles and/or SVG definitions under SVG <defs/>."""
+    if css_styles is None or svg_definitions is None:
+        return original
+
+    insertion_point = original.find("</defs>")
+    text_css = (
+        css_styles.read_text() if isinstance(css_styles, Path) else css_styles
+    )
+    return (
+        f"{original[:insertion_point]}"
+        f"{svg_definitions or ''}\n"
+        f'<style type="text/css">\n{text_css}</style>\n'
+        f" {original[insertion_point:]}"
+    )
```

### Comparing `psychrochart-0.8.0/pyproject.toml` & `psychrochart-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 log_level = "INFO"
 log_cli = true
 log_format = "%(asctime)s %(levelname)s: (%(filename)s:%(lineno)s): %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.poetry]
 name = "psychrochart"
-version = "0.8.0"
+version = "0.9.0"
 description = "A python 3 library to make psychrometric charts and overlay information on them"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 packages = [
     { include = "psychrochart" }
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `psychrochart-0.8.0/PKG-INFO` & `psychrochart-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychrochart
-Version: 0.8.0
+Version: 0.9.0
 Summary: A python 3 library to make psychrometric charts and overlay information on them
 Home-page: https://github.com/azogue/psychrochart
 License: MIT
 Keywords: psychrometrics,moist,humid air,climate control,matplotlib
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
 Requires-Python: >=3.10,<3.12
```

