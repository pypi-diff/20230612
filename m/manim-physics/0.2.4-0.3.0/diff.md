# Comparing `tmp/manim-physics-0.2.4.tar.gz` & `tmp/manim_physics-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim-physics-0.2.4.tar", max compression
+gzip compressed data, was "manim_physics-0.3.0.tar", max compression
```

## Comparing `manim-physics-0.2.4.tar` & `manim_physics-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0      559 2022-03-03 10:48:00.842108 manim-physics-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     9985 2022-03-02 11:16:42.599502 manim-physics-0.2.4/README.md
--rw-r--r--   0        0        0      160 2022-02-27 13:32:11.875314 manim-physics-0.2.4/src/manim_physics/__init__.py
--rw-r--r--   0        0        0    10946 2022-03-03 10:47:56.880807 manim-physics-0.2.4/src/manim_physics/electromagnetism.py
--rw-r--r--   0        0        0     7668 2022-03-03 10:47:56.825847 manim-physics-0.2.4/src/manim_physics/lensing.py
--rw-r--r--   0        0        0     5049 2022-02-27 13:32:11.878315 manim-physics-0.2.4/src/manim_physics/pendulum.py
--rw-r--r--   0        0        0     7965 2022-03-03 10:47:56.791839 manim-physics-0.2.4/src/manim_physics/rigid_mechanics.py
--rw-r--r--   0        0        0     7589 2022-03-03 10:47:56.790839 manim-physics-0.2.4/src/manim_physics/wave.py
--rw-r--r--   0        0        0    10856 2022-03-03 10:51:20.487442 manim-physics-0.2.4/setup.py
--rw-r--r--   0        0        0    10367 2022-03-03 10:51:20.488442 manim-physics-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      301 2023-06-12 03:32:54.254775 manim_physics-0.3.0/manim_physics/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:32:54.255761 manim_physics-0.3.0/manim_physics/electromagnetism/__init__.py
+-rw-r--r--   0        0        0     4496 2023-06-12 03:32:54.256759 manim_physics-0.3.0/manim_physics/electromagnetism/electrostatics.py
+-rw-r--r--   0        0        0     3043 2023-06-12 03:32:54.257756 manim_physics-0.3.0/manim_physics/electromagnetism/magnetostatics.py
+-rw-r--r--   0        0        0      108 2023-06-12 03:32:54.258762 manim_physics-0.3.0/manim_physics/optics/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-12 03:32:54.259756 manim_physics-0.3.0/manim_physics/optics/lenses.py
+-rw-r--r--   0        0        0     5026 2023-06-12 03:32:54.260751 manim_physics-0.3.0/manim_physics/optics/rays.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:32:54.260751 manim_physics-0.3.0/manim_physics/rigid_mechanics/__init__.py
+-rw-r--r--   0        0        0     5267 2023-06-12 03:32:54.261771 manim_physics-0.3.0/manim_physics/rigid_mechanics/pendulum.py
+-rw-r--r--   0        0        0     7977 2023-06-12 03:32:54.262758 manim_physics-0.3.0/manim_physics/rigid_mechanics/rigid_mechanics.py
+-rw-r--r--   0        0        0     7381 2023-06-12 03:32:54.263759 manim_physics-0.3.0/manim_physics/wave.py
+-rw-r--r--   0        0        0      760 2023-06-12 03:33:16.999818 manim_physics-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      711 2023-06-12 03:32:54.237754 manim_physics-0.3.0/README.md
+-rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 manim_physics-0.3.0/setup.py
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 manim_physics-0.3.0/PKG-INFO
```

### Comparing `manim-physics-0.2.4/src/manim_physics/rigid_mechanics.py` & `manim_physics-0.3.0/manim_physics/rigid_mechanics/rigid_mechanics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,234 +1,241 @@
-"""A gravity simulation space.
-
-Most objects can be made into a rigid body (moves according to gravity
-and collision) or a static body (stays still within the scene).
-
-To use this feature, the :class:`~SpaceScene` must be used, to access
-the specific functions of the space.
-
-.. note::
-    *   This feature utilizes the pymunk package. Although unnecessary,
-        it might make it easier if you knew a few things on how to use it.
-
-        `Official Documentation <http://www.pymunk.org/en/latest/pymunk.html>`_
-
-        `Youtube Tutorial <https://youtu.be/pRk---rdrbo>`_
-
-    *   A low frame rate might cause some objects to pass static objects as
-        they don't register collisions finely enough. Trying to increase the
-        config frame rate might solve the problem.
-
-Examples
---------
-.. manim:: TwoObjectsFalling
-        
-        from manim_physics import *
-        # use a SpaceScene to utilize all specific rigid-mechanics methods
-        class TwoObjectsFalling(SpaceScene):
-            def construct(self):
-                circle = Circle().shift(UP)
-                circle.set_fill(RED, 1)
-                circle.shift(DOWN + RIGHT)
-
-                rect = Square().shift(UP)
-                rect.rotate(PI / 4)
-                rect.set_fill(YELLOW_A, 1)
-                rect.shift(UP * 2)
-                rect.scale(0.5)
-
-                ground = Line([-4, -3.5, 0], [4, -3.5, 0])
-                wall1 = Line([-4, -3.5, 0], [-4, 3.5, 0])
-                wall2 = Line([4, -3.5, 0], [4, 3.5, 0])
-                walls = VGroup(ground, wall1, wall2)
-                self.add(walls)
-
-                self.play(
-                    DrawBorderThenFill(circle),
-                    DrawBorderThenFill(rect),
-                )
-                self.make_rigid_body(rect, circle)  # Mobjects will move with gravity
-                self.make_static_body(walls)  # Mobjects will stay in place
-                self.wait(5)
-                # during wait time, the circle and rect would move according to the simulate updater
-"""
-
-__all__ = [
-    "Space",
-    "_step",
-    "_simulate",
-    "get_shape",
-    "get_angle",
-    "SpaceScene",
-]
-
-from typing import Tuple
-import pymunk
-from manim import *
-
-try:
-    # For manim < 0.15.0
-    from manim.mobject.opengl_compatibility import ConvertToOpenGL
-except ModuleNotFoundError:
-    # For manim >= 0.15.0
-    from manim.mobject.opengl.opengl_compatibility import ConvertToOpenGL
-
-
-class Space(Mobject, metaclass=ConvertToOpenGL):
-    def __init__(self, gravity: Tuple[float, float] = (0, -9.81), **kwargs):
-        """An Abstract object for gravity.
-
-        Parameters
-        ----------
-        gravity
-            The direction and strength of gravity.
-        """
-        super().__init__(**kwargs)
-        self.space = pymunk.Space()
-        self.space.gravity = gravity
-        self.space.sleep_time_threshold = 5
-
-
-class SpaceScene(Scene):
-    GRAVITY: Tuple[float, float] = 0, -9.81
-
-    def __init__(self, renderer=None, **kwargs):
-        """A basis scene for all of rigid mechanics. The gravity vector
-        can be adjusted with ``self.GRAVITY``.
-        """
-        self.space = Space(gravity=self.GRAVITY)
-        super().__init__(renderer=renderer, **kwargs)
-
-    def setup(self):
-        """Used internally"""
-        self.add(self.space)
-        self.space.add_updater(_step)
-
-    def add_body(self, body: Mobject):
-        """Bodies refer to pymunk's object.
-        This method ties Mobjects to their Bodies.
-        """
-        if body.body != self.space.space.static_body:
-            self.space.space.add(body.body)
-        self.space.space.add(body.shape)
-
-    def make_rigid_body(
-        self,
-        *mobs: Mobject,
-        elasticity: float = 0.8,
-        density: float = 1,
-        friction: float = 0.8,
-    ):
-        """Make any mobject movable by gravity.
-        Equivalent to ``Scene``'s ``add`` function.
-
-        Parameters
-        ----------
-        mobs
-            The mobs to be made rigid.
-        elasticity
-        density
-        friction
-            The attributes of the mobjects in regards to
-            interacting with other rigid and static objects.
-        """
-        for mob in mobs:
-            if isinstance(mob, VGroup):
-                return self.make_rigid_body(*mob)
-            if not hasattr(mob, "body"):
-                parts = mob.family_members_with_points()
-                for p in parts:
-                    self.add(p)
-                    p.body = pymunk.Body()
-                    p.body.position = p.get_x(), p.get_y()
-                    get_angle(p)
-                    if not hasattr(p, "angle"):
-                        p.angle = 0
-                    p.body.angle = p.angle
-                    get_shape(p)
-                    p.shape.density = density
-                    p.shape.elasticity = elasticity
-                    p.shape.friction = friction
-                    p.spacescene = self
-
-                    self.add_body(p)
-                    p.add_updater(_simulate)
-
-            else:
-                if mob.body.is_sleeping:
-                    mob.body.activate()
-
-    def make_static_body(
-        self, *mobs: Mobject, elasticity: float = 1, friction: float = 0.8
-    ) -> None:
-        """Make any mobject interactable by rigid objects.
-
-        Parameters
-        ----------
-        mobs
-            The mobs to be made static.
-        elasticity
-        friction
-            The attributes of the mobjects in regards to
-            interacting with rigid objects.
-        """
-        for mob in mobs:
-            if isinstance(mob, VGroup or Group):
-                return self.make_static_body(*mob)
-            mob.body = self.space.space.static_body
-            get_shape(mob)
-            mob.shape.elasticity = elasticity
-            mob.shape.friction = friction
-            self.add_body(mob)
-
-    def stop_rigidity(self, *mobs: Mobject) -> None:
-        """Stop the mobjects rigidity"""
-        for mob in mobs:
-            if isinstance(mob, VGroup or Group):
-                self.stop_rigidity(*mob)
-            if hasattr(mob, "body"):
-                mob.body.sleep()
-
-
-def _step(space, dt):
-    space.space.step(dt)
-
-
-def _simulate(b):
-    x, y = b.body.position
-    b.move_to(x * RIGHT + y * UP)
-    b.rotate(b.body.angle - b.angle)
-    b.angle = b.body.angle
-
-
-def get_shape(mob: VMobject) -> None:
-    """Obtains the shape of the body from the mobject"""
-    if isinstance(mob, Circle):
-        mob.shape = pymunk.Circle(body=mob.body, radius=mob.radius)
-    elif isinstance(mob, Line):
-        mob.shape = pymunk.Segment(
-            mob.body,
-            (mob.get_start()[0], mob.get_start()[1]),
-            (mob.get_end()[0], mob.get_end()[1]),
-            mob.stroke_width - 3.95,
-        )
-    elif issubclass(type(mob), Rectangle):
-        width = np.linalg.norm(mob.get_vertices()[1] - mob.get_vertices()[0])
-        height = np.linalg.norm(mob.get_vertices()[2] - mob.get_vertices()[1])
-        mob.shape = pymunk.Poly.create_box(mob.body, (width, height))
-    elif issubclass(type(mob), Polygram):
-        vertices = [(a, b) for a, b, c in mob.get_vertices() - mob.get_center()]
-        mob.shape = pymunk.Poly(mob.body, vertices)
-    else:
-        mob.shape = pymunk.Poly.create_box(mob.body, (mob.width, mob.height))
-
-
-def get_angle(mob: VMobject) -> None:
-    """Obtains the angle of the body from the mobject.
-    Used internally for updaters.
-    """
-    if issubclass(type(mob), Polygon):
-        vec1 = mob.get_vertices()[0] - mob.get_vertices()[1]
-        vec2 = type(mob)().get_vertices()[0] - type(mob)().get_vertices()[1]
-        mob.angle = angle_between_vectors(vec1, vec2)
-    elif isinstance(mob, Line):
-        mob.angle = mob.get_angle()
+"""A gravity simulation space.
+
+Most objects can be made into a rigid body (moves according to gravity
+and collision) or a static body (stays still within the scene).
+
+To use this feature, the :class:`~SpaceScene` must be used, to access
+the specific functions of the space.
+
+.. note::
+    *   This feature utilizes the pymunk package. Although unnecessary,
+        it might make it easier if you knew a few things on how to use it.
+
+        `Official Documentation <http://www.pymunk.org/en/latest/pymunk.html>`_
+
+        `Youtube Tutorial <https://youtu.be/pRk---rdrbo>`_
+
+    *   A low frame rate might cause some objects to pass static objects as
+        they don't register collisions finely enough. Trying to increase the
+        config frame rate might solve the problem.
+
+Examples
+--------
+.. manim:: TwoObjectsFalling
+        
+        from manim_physics import *
+        # use a SpaceScene to utilize all specific rigid-mechanics methods
+        class TwoObjectsFalling(SpaceScene):
+            def construct(self):
+                circle = Circle().shift(UP)
+                circle.set_fill(RED, 1)
+                circle.shift(DOWN + RIGHT)
+
+                rect = Square().shift(UP)
+                rect.rotate(PI / 4)
+                rect.set_fill(YELLOW_A, 1)
+                rect.shift(UP * 2)
+                rect.scale(0.5)
+
+                ground = Line([-4, -3.5, 0], [4, -3.5, 0])
+                wall1 = Line([-4, -3.5, 0], [-4, 3.5, 0])
+                wall2 = Line([4, -3.5, 0], [4, 3.5, 0])
+                walls = VGroup(ground, wall1, wall2)
+                self.add(walls)
+
+                self.play(
+                    DrawBorderThenFill(circle),
+                    DrawBorderThenFill(rect),
+                )
+                self.make_rigid_body(rect, circle)  # Mobjects will move with gravity
+                self.make_static_body(walls)  # Mobjects will stay in place
+                self.wait(5)
+                # during wait time, the circle and rect would move according to the simulate updater
+"""
+
+from __future__ import annotations
+from typing import Tuple
+
+from manim.constants import RIGHT, UP
+from manim.mobject.geometry.arc import Circle
+from manim.mobject.geometry.line import Line
+from manim.mobject.geometry.polygram import Polygon, Polygram, Rectangle
+from manim.mobject.mobject import Group, Mobject
+from manim.mobject.types.vectorized_mobject import VGroup, VMobject
+from manim.scene.scene import Scene
+from manim.utils.space_ops import angle_between_vectors
+import numpy as np
+import pymunk
+
+__all__ = [
+    "Space",
+    "_step",
+    "_simulate",
+    "get_shape",
+    "get_angle",
+    "SpaceScene",
+]
+
+
+try:
+    # For manim < 0.15.0
+    from manim.mobject.opengl_compatibility import ConvertToOpenGL
+except ModuleNotFoundError:
+    # For manim >= 0.15.0
+    from manim.mobject.opengl.opengl_compatibility import ConvertToOpenGL
+
+
+class Space(Mobject, metaclass=ConvertToOpenGL):
+    def __init__(self, gravity: Tuple[float, float] = (0, -9.81), **kwargs):
+        """An Abstract object for gravity.
+
+        Parameters
+        ----------
+        gravity
+            The direction and strength of gravity.
+        """
+        super().__init__(**kwargs)
+        self.space = pymunk.Space()
+        self.space.gravity = gravity
+        self.space.sleep_time_threshold = 5
+
+
+class SpaceScene(Scene):
+    GRAVITY: Tuple[float, float] = 0, -9.81
+
+    def __init__(self, renderer=None, **kwargs):
+        """A basis scene for all of rigid mechanics. The gravity vector
+        can be adjusted with ``self.GRAVITY``.
+        """
+        self.space = Space(gravity=self.GRAVITY)
+        super().__init__(renderer=renderer, **kwargs)
+
+    def setup(self):
+        """Used internally"""
+        self.add(self.space)
+        self.space.add_updater(_step)
+
+    def add_body(self, body: Mobject):
+        """Bodies refer to pymunk's object.
+        This method ties Mobjects to their Bodies.
+        """
+        if body.body != self.space.space.static_body:
+            self.space.space.add(body.body)
+        self.space.space.add(body.shape)
+
+    def make_rigid_body(
+        self,
+        *mobs: Mobject,
+        elasticity: float = 0.8,
+        density: float = 1,
+        friction: float = 0.8,
+    ):
+        """Make any mobject movable by gravity.
+        Equivalent to ``Scene``'s ``add`` function.
+
+        Parameters
+        ----------
+        mobs
+            The mobs to be made rigid.
+        elasticity
+        density
+        friction
+            The attributes of the mobjects in regards to
+            interacting with other rigid and static objects.
+        """
+        for mob in mobs:
+            if not hasattr(mob, "body"):
+                self.add(mob)
+                mob.body = pymunk.Body()
+                mob.body.position = mob.get_x(), mob.get_y()
+                get_angle(mob)
+                if not hasattr(mob, "angle"):
+                    mob.angle = 0
+                mob.body.angle = mob.angle
+                get_shape(mob)
+                mob.shape.density = density
+                mob.shape.elasticity = elasticity
+                mob.shape.friction = friction
+                mob.spacescene = self
+
+                self.add_body(mob)
+                mob.add_updater(_simulate)
+
+            else:
+                if mob.body.is_sleeping:
+                    mob.body.activate()
+
+    def make_static_body(
+        self, *mobs: Mobject, elasticity: float = 1, friction: float = 0.8
+    ) -> None:
+        """Make any mobject interactable by rigid objects.
+
+        Parameters
+        ----------
+        mobs
+            The mobs to be made static.
+        elasticity
+        friction
+            The attributes of the mobjects in regards to
+            interacting with rigid objects.
+        """
+        for mob in mobs:
+            if isinstance(mob, VGroup or Group):
+                return self.make_static_body(*mob)
+            mob.body = self.space.space.static_body
+            get_shape(mob)
+            mob.shape.elasticity = elasticity
+            mob.shape.friction = friction
+            self.add_body(mob)
+
+    def stop_rigidity(self, *mobs: Mobject) -> None:
+        """Stop the mobjects rigidity"""
+        for mob in mobs:
+            if isinstance(mob, VGroup or Group):
+                self.stop_rigidity(*mob)
+            if hasattr(mob, "body"):
+                mob.body.sleep()
+
+
+def _step(space, dt):
+    space.space.step(dt)
+
+
+def _simulate(b):
+    x, y = b.body.position
+    b.move_to(x * RIGHT + y * UP)
+    b.rotate(b.body.angle - b.angle)
+    b.angle = b.body.angle
+
+
+def get_shape(mob: VMobject) -> None:
+    """Obtains the shape of the body from the mobject"""
+    if isinstance(mob, Circle):
+        mob.shape = pymunk.Circle(body=mob.body, radius=mob.radius)
+    elif isinstance(mob, Line):
+        mob.shape = pymunk.Segment(
+            mob.body,
+            (mob.get_start()[0], mob.get_start()[1]),
+            (mob.get_end()[0], mob.get_end()[1]),
+            mob.stroke_width - 3.95,
+        )
+    elif issubclass(type(mob), Rectangle):
+        width = np.linalg.norm(mob.get_vertices()[1] - mob.get_vertices()[0])
+        height = np.linalg.norm(mob.get_vertices()[2] - mob.get_vertices()[1])
+        mob.shape = pymunk.Poly.create_box(mob.body, (width, height))
+    elif issubclass(type(mob), Polygram):
+        vertices = [(a, b) for a, b, _ in mob.get_vertices() - mob.get_center()]
+        mob.shape = pymunk.Poly(mob.body, vertices)
+    else:
+        mob.shape = pymunk.Poly.create_box(mob.body, (mob.width, mob.height))
+
+
+def get_angle(mob: VMobject) -> None:
+    """Obtains the angle of the body from the mobject.
+    Used internally for updaters.
+    """
+    if issubclass(type(mob), Polygon):
+        vec1 = mob.get_vertices()[0] - mob.get_vertices()[1]
+        vec2 = type(mob)().get_vertices()[0] - type(mob)().get_vertices()[1]
+        mob.angle = angle_between_vectors(vec1, vec2)
+    elif isinstance(mob, Line):
+        mob.angle = mob.get_angle()
```

### Comparing `manim-physics-0.2.4/src/manim_physics/wave.py` & `manim_physics-0.3.0/manim_physics/wave.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,248 +1,251 @@
-"""3D and 2D Waves module."""
-
-__all__ = [
-    "LinearWave",
-    "RadialWave",
-    "StandingWave",
-]
-
-from typing import Iterable, Optional
-from manim import *
-
-try:
-    # For manim < 0.15.0
-    from manim.mobject.opengl_compatibility import ConvertToOpenGL
-except ModuleNotFoundError:
-    # For manim >= 0.15.0
-    from manim.mobject.opengl.opengl_compatibility import ConvertToOpenGL
-
-
-class RadialWave(Surface, metaclass=ConvertToOpenGL):
-    def __init__(
-        self,
-        *sources: Optional[np.ndarray],
-        wavelength: float = 1,
-        period: float = 1,
-        amplitude: float = 0.1,
-        x_range: Iterable[float] = [-5, 5],
-        y_range: Iterable[float] = [-5, 5],
-        **kwargs
-    ) -> None:
-        """A 3D Surface with waves moving radially.
-
-        Parameters
-        ----------
-        sources
-            The sources of disturbance.
-        wavelength
-            The wavelength of the wave.
-        period
-            The period of the wave.
-        amplitude
-            The amplitude of the wave.
-        x_range
-            The range of the wave in the x direction.
-        y_range
-            The range of the wave in the y direction.
-        kwargs
-            Additional parameters to be passed to :class:`~Surface`.
-
-        Examples
-        --------
-        .. manim:: RadialWaveExampleScene
-
-            class RadialWaveExampleScene(ThreeDScene):
-                def construct(self):
-                    self.set_camera_orientation(60 * DEGREES, -45 * DEGREES)
-                    wave = RadialWave(
-                        LEFT * 2 + DOWN * 5,  # Two source of waves
-                        RIGHT * 2 + DOWN * 5,
-                        checkerboard_colors=[BLUE_D],
-                        stroke_width=0,
-                    )
-                    self.add(wave)
-                    wave.start_wave()
-                    self.wait()
-                    wave.stop_wave()
-        """
-        self.wavelength = wavelength
-        self.period = period
-        self.amplitude = amplitude
-        self.time = 0
-        self.kwargs = kwargs
-        self.sources = sources
-
-        super().__init__(
-            lambda u, v: np.array([u, v, self._wave_z(u, v, sources)]),
-            u_range=x_range,
-            v_range=y_range,
-            **kwargs,
-        )
-
-    def _wave_z(self, u: float, v: float, sources: Iterable[np.ndarray]) -> float:
-        z = 0
-        for source in sources:
-            x0, y0, _ = source
-            z += self.amplitude * np.sin(
-                (2 * PI / self.wavelength) * ((u - x0) ** 2 + (v - y0) ** 2) ** 0.5
-                - 2 * PI * self.time / self.period
-            )
-        return z
-
-    def _update_wave(self, mob: Mobject, dt: float) -> None:
-        self.time += dt
-        mob.match_points(
-            Surface(
-                lambda u, v: np.array([u, v, self._wave_z(u, v, self.sources)]),
-                u_range=self.u_range,
-                v_range=self.v_range,
-                **self.kwargs,
-            )
-        )
-
-    def start_wave(self):
-        """Animate the wave propagation."""
-        self.add_updater(self._update_wave)
-
-    def stop_wave(self):
-        """Stop animating the wave propagation."""
-        self.remove_updater(self._update_wave)
-
-
-class LinearWave(RadialWave):
-    def __init__(
-        self,
-        wavelength: float = 1,
-        period: float = 1,
-        amplitude: float = 0.1,
-        x_range: Iterable[float] = [-5, 5],
-        y_range: Iterable[float] = [-5, 5],
-        **kwargs
-    ) -> None:
-        """A 3D Surface with waves in one direction.
-
-        Parameters
-        ----------
-        wavelength
-            The wavelength of the wave.
-        period
-            The period of the wave.
-        amplitude
-            The amplitude of the wave.
-        x_range
-            The range of the wave in the x direction.
-        y_range
-            The range of the wave in the y direction.
-        kwargs
-            Additional parameters to be passed to :class:`~Surface`.
-
-        Examples
-        --------
-        .. manim:: LinearWaveExampleScene
-
-            class LinearWaveExampleScene(ThreeDScene):
-                def construct(self):
-                    self.set_camera_orientation(60 * DEGREES, -45 * DEGREES)
-                    wave = LinearWave()
-                    self.add(wave)
-                    wave.start_wave()
-                    self.wait()
-                    wave.stop_wave()
-        """
-        super().__init__(
-            ORIGIN,
-            wavelength=wavelength,
-            period=period,
-            amplitude=amplitude,
-            x_range=x_range,
-            y_range=y_range,
-            **kwargs,
-        )
-
-    def _wave_z(self, u: float, v: float, sources: Iterable[np.ndarray]) -> float:
-        return self.amplitude * np.sin(
-            (2 * PI / self.wavelength) * u - 2 * PI * self.time / self.period
-        )
-
-
-class StandingWave(ParametricFunction):
-    def __init__(
-        self,
-        n: int = 2,
-        length: float = 4,
-        period: float = 1,
-        amplitude: float = 1,
-        **kwargs
-    ) -> None:
-        """A 2D standing wave.
-
-        Parameters
-        ----------
-        n
-            Harmonic number.
-        length
-            The length of the wave.
-        period
-            The time taken for one full oscillation.
-        amplitude
-            The maximum height of the wave.
-        kwargs
-            Additional parameters to be passed to :class:`~ParametricFunction`.
-
-        Examples
-        --------
-        .. manim:: StandingWaveExampleScene
-
-            from manim_physics import *
-
-            class StandingWaveExampleScene(Scene):
-                def construct(self):
-                    wave1 = StandingWave(1)
-                    wave2 = StandingWave(2)
-                    wave3 = StandingWave(3)
-                    wave4 = StandingWave(4)
-                    waves = VGroup(wave1, wave2, wave3, wave4)
-                    waves.arrange(DOWN).move_to(ORIGIN)
-                    self.add(waves)
-                    for wave in waves:
-                        wave.start_wave()
-                    self.wait()
-        """
-        self.n = n
-        self.length = length
-        self.period = period
-        self.amplitude = amplitude
-        self.time = 0
-        self.kwargs = {**kwargs}
-
-        super().__init__(
-            lambda t: np.array([t, amplitude * np.sin(n * PI * t / length), 0]),
-            t_range=[0, length],
-            **kwargs,
-        )
-        self.shift([-self.length / 2, 0, 0])
-
-    def _update_wave(self, mob: Mobject, dt: float) -> None:
-        self.time += dt
-        mob.become(
-            ParametricFunction(
-                lambda t: np.array(
-                    [
-                        t,
-                        self.amplitude
-                        * np.sin(self.n * PI * t / self.length)
-                        * np.cos(2 * PI * self.time / self.period),
-                        0,
-                    ]
-                ),
-                t_range=[0, self.length],
-                **self.kwargs,
-            ).shift(self.wave_center + [-self.length / 2, 0, 0])
-        )
-
-    def start_wave(self):
-        self.wave_center = self.get_center()
-        self.add_updater(self._update_wave)
-
-    def stop_wave(self):
-        self.remove_updater(self._update_wave)
+"""3D and 2D Waves module."""
+
+from __future__ import annotations
+from typing import Iterable, Optional
+
+from manim import *
+
+__all__ = [
+    "LinearWave",
+    "RadialWave",
+    "StandingWave",
+]
+
+
+try:
+    # For manim < 0.15.0
+    from manim.mobject.opengl_compatibility import ConvertToOpenGL
+except ModuleNotFoundError:
+    # For manim >= 0.15.0
+    from manim.mobject.opengl.opengl_compatibility import ConvertToOpenGL
+
+
+class RadialWave(Surface, metaclass=ConvertToOpenGL):
+    def __init__(
+        self,
+        *sources: Optional[np.ndarray],
+        wavelength: float = 1,
+        period: float = 1,
+        amplitude: float = 0.1,
+        x_range: Iterable[float] = [-5, 5],
+        y_range: Iterable[float] = [-5, 5],
+        **kwargs,
+    ) -> None:
+        """A 3D Surface with waves moving radially.
+
+        Parameters
+        ----------
+        sources
+            The sources of disturbance.
+        wavelength
+            The wavelength of the wave.
+        period
+            The period of the wave.
+        amplitude
+            The amplitude of the wave.
+        x_range
+            The range of the wave in the x direction.
+        y_range
+            The range of the wave in the y direction.
+        kwargs
+            Additional parameters to be passed to :class:`~Surface`.
+
+        Examples
+        --------
+        .. manim:: RadialWaveExampleScene
+
+            class RadialWaveExampleScene(ThreeDScene):
+                def construct(self):
+                    self.set_camera_orientation(60 * DEGREES, -45 * DEGREES)
+                    wave = RadialWave(
+                        LEFT * 2 + DOWN * 5,  # Two source of waves
+                        RIGHT * 2 + DOWN * 5,
+                        checkerboard_colors=[BLUE_D],
+                        stroke_width=0,
+                    )
+                    self.add(wave)
+                    wave.start_wave()
+                    self.wait()
+                    wave.stop_wave()
+        """
+        self.wavelength = wavelength
+        self.period = period
+        self.amplitude = amplitude
+        self.time = 0
+        self.kwargs = kwargs
+        self.sources = sources
+
+        super().__init__(
+            lambda u, v: np.array([u, v, self._wave_z(u, v, sources)]),
+            u_range=x_range,
+            v_range=y_range,
+            **kwargs,
+        )
+
+    def _wave_z(self, u: float, v: float, sources: Iterable[np.ndarray]) -> float:
+        z = 0
+        for source in sources:
+            x0, y0, _ = source
+            z += self.amplitude * np.sin(
+                (2 * PI / self.wavelength) * ((u - x0) ** 2 + (v - y0) ** 2) ** 0.5
+                - 2 * PI * self.time / self.period
+            )
+        return z
+
+    def _update_wave(self, mob: Mobject, dt: float) -> None:
+        self.time += dt
+        mob.match_points(
+            Surface(
+                lambda u, v: np.array([u, v, self._wave_z(u, v, self.sources)]),
+                u_range=self.u_range,
+                v_range=self.v_range,
+                **self.kwargs,
+            )
+        )
+
+    def start_wave(self):
+        """Animate the wave propagation."""
+        self.add_updater(self._update_wave)
+
+    def stop_wave(self):
+        """Stop animating the wave propagation."""
+        self.remove_updater(self._update_wave)
+
+
+class LinearWave(RadialWave):
+    def __init__(
+        self,
+        wavelength: float = 1,
+        period: float = 1,
+        amplitude: float = 0.1,
+        x_range: Iterable[float] = [-5, 5],
+        y_range: Iterable[float] = [-5, 5],
+        **kwargs,
+    ) -> None:
+        """A 3D Surface with waves in one direction.
+
+        Parameters
+        ----------
+        wavelength
+            The wavelength of the wave.
+        period
+            The period of the wave.
+        amplitude
+            The amplitude of the wave.
+        x_range
+            The range of the wave in the x direction.
+        y_range
+            The range of the wave in the y direction.
+        kwargs
+            Additional parameters to be passed to :class:`~Surface`.
+
+        Examples
+        --------
+        .. manim:: LinearWaveExampleScene
+
+            class LinearWaveExampleScene(ThreeDScene):
+                def construct(self):
+                    self.set_camera_orientation(60 * DEGREES, -45 * DEGREES)
+                    wave = LinearWave()
+                    self.add(wave)
+                    wave.start_wave()
+                    self.wait()
+                    wave.stop_wave()
+        """
+        super().__init__(
+            ORIGIN,
+            wavelength=wavelength,
+            period=period,
+            amplitude=amplitude,
+            x_range=x_range,
+            y_range=y_range,
+            **kwargs,
+        )
+
+    def _wave_z(self, u: float, v: float, sources: Iterable[np.ndarray]) -> float:
+        return self.amplitude * np.sin(
+            (2 * PI / self.wavelength) * u - 2 * PI * self.time / self.period
+        )
+
+
+class StandingWave(ParametricFunction):
+    def __init__(
+        self,
+        n: int = 2,
+        length: float = 4,
+        period: float = 1,
+        amplitude: float = 1,
+        **kwargs,
+    ) -> None:
+        """A 2D standing wave.
+
+        Parameters
+        ----------
+        n
+            Harmonic number.
+        length
+            The length of the wave.
+        period
+            The time taken for one full oscillation.
+        amplitude
+            The maximum height of the wave.
+        kwargs
+            Additional parameters to be passed to :class:`~ParametricFunction`.
+
+        Examples
+        --------
+        .. manim:: StandingWaveExampleScene
+
+            from manim_physics import *
+
+            class StandingWaveExampleScene(Scene):
+                def construct(self):
+                    wave1 = StandingWave(1)
+                    wave2 = StandingWave(2)
+                    wave3 = StandingWave(3)
+                    wave4 = StandingWave(4)
+                    waves = VGroup(wave1, wave2, wave3, wave4)
+                    waves.arrange(DOWN).move_to(ORIGIN)
+                    self.add(waves)
+                    for wave in waves:
+                        wave.start_wave()
+                    self.wait()
+        """
+        self.n = n
+        self.length = length
+        self.period = period
+        self.amplitude = amplitude
+        self.time = 0
+        self.kwargs = {**kwargs}
+
+        super().__init__(
+            lambda t: np.array([t, amplitude * np.sin(n * PI * t / length), 0]),
+            t_range=[0, length],
+            **kwargs,
+        )
+        self.shift([-self.length / 2, 0, 0])
+
+    def _update_wave(self, mob: Mobject, dt: float) -> None:
+        self.time += dt
+        mob.become(
+            ParametricFunction(
+                lambda t: np.array(
+                    [
+                        t,
+                        self.amplitude
+                        * np.sin(self.n * PI * t / self.length)
+                        * np.cos(2 * PI * self.time / self.period),
+                        0,
+                    ]
+                ),
+                t_range=[0, self.length],
+                **self.kwargs,
+            ).shift(self.wave_center + [-self.length / 2, 0, 0])
+        )
+
+    def start_wave(self):
+        self.wave_center = self.get_center()
+        self.add_updater(self._update_wave)
+
+    def stop_wave(self):
+        self.remove_updater(self._update_wave)
```

