# Comparing `tmp/jaxrenderer-0.2.1.tar.gz` & `tmp/jaxrenderer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrenderer-0.2.1.tar", max compression
+gzip compressed data, was "jaxrenderer-0.3.0.tar", max compression
```

## Comparing `jaxrenderer-0.2.1.tar` & `jaxrenderer-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    11367 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/LICENSE
--rw-r--r--   0        0        0     2312 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/README.md
--rw-r--r--   0        0        0     4797 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/changelog.md
--rw-r--r--   0        0        0     1540 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4851 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/renderer/README.md
--rw-r--r--   0        0        0      539 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/renderer/__init__.py
--rw-r--r--   0        0        0    33725 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/renderer/geometry.py
--rw-r--r--   0        0        0    17155 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/renderer/model.py
--rw-r--r--   0        0        0    13911 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/pipeline.py
--rw-r--r--   0        0        0    13883 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/renderer.py
--rw-r--r--   0        0        0     9130 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/scene.py
--rw-r--r--   0        0        0    10102 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shader.py
--rw-r--r--   0        0        0     4600 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/README.md
--rw-r--r--   0        0        0     1256 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/depth.py
--rw-r--r--   0        0        0     3252 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/gouraud.py
--rw-r--r--   0        0        0     4804 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/gouraud_texture.py
--rw-r--r--   0        0        0     5079 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/phong.py
--rw-r--r--   0        0        0     9571 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/phong_darboux.py
--rw-r--r--   0        0        0     7926 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/phong_reflection.py
--rw-r--r--   0        0        0     9650 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/phong_reflection_shadow.py
--rw-r--r--   0        0        0     4166 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shadow.py
--rw-r--r--   0        0        0    71549 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shapes/capsule.py
--rw-r--r--   0        0        0     3574 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shapes/cube.py
--rw-r--r--   0        0        0     3270 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/types.py
--rw-r--r--   0        0        0     3074 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/utils.py
--rw-r--r--   0        0        0      833 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/value_checker.py
--rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 jaxrenderer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11367 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2312 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/README.md
+-rw-r--r--   0        0        0     5935 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/changelog.md
+-rw-r--r--   0        0        0     1559 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5637 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/README.md
+-rw-r--r--   0        0        0      539 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/__init__.py
+-rw-r--r--   0        0        0      741 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/_meta_utils.py
+-rw-r--r--   0        0        0    34989 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/geometry.py
+-rw-r--r--   0        0        0    17431 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/model.py
+-rw-r--r--   0        0        0    17457 2023-06-12 09:03:18.232993 jaxrenderer-0.3.0/renderer/pipeline.py
+-rw-r--r--   0        0        0    14617 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/renderer.py
+-rw-r--r--   0        0        0     9130 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/scene.py
+-rw-r--r--   0        0        0    14563 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shader.py
+-rw-r--r--   0        0        0     4600 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/README.md
+-rw-r--r--   0        0        0     1373 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/depth.py
+-rw-r--r--   0        0        0     3413 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/gouraud.py
+-rw-r--r--   0        0        0     5009 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/gouraud_texture.py
+-rw-r--r--   0        0        0     5284 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/phong.py
+-rw-r--r--   0        0        0     9820 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/phong_darboux.py
+-rw-r--r--   0        0        0     8035 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/phong_reflection.py
+-rw-r--r--   0        0        0     9759 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shaders/phong_reflection_shadow.py
+-rw-r--r--   0        0        0     4517 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shadow.py
+-rw-r--r--   0        0        0    71549 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shapes/capsule.py
+-rw-r--r--   0        0        0     3574 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/shapes/cube.py
+-rw-r--r--   0        0        0     3270 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/types.py
+-rw-r--r--   0        0        0     3284 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/utils.py
+-rw-r--r--   0        0        0      833 2023-06-12 09:03:18.236992 jaxrenderer-0.3.0/renderer/value_checker.py
+-rw-r--r--   0        0        0     3719 1970-01-01 00:00:00.000000 jaxrenderer-0.3.0/PKG-INFO
```

### Comparing `jaxrenderer-0.2.1/LICENSE` & `jaxrenderer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.1/README.md` & `jaxrenderer-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.1/changelog.md` & `jaxrenderer-0.3.0/changelog.md`

 * *Files 16% similar despite different names*

```diff
@@ -45,7 +45,15 @@
 1. Instead of clipping (planned to be implemented), now the rasteriser interpolates in homogeneous space directly. `Shader.interpolate` will not receive valid `barycentric_screen` values for now. Setting `Interpolation.SMOOTH` and `Interpolation.NOPERSPECTIVE` will result in same results, perspective-correct interpolations.
 2. Reorganise example files and rename them.
 
 ## 0.2.1
 
 1. Refactor `Scene.set_object_*` methods to be a simple wrapper of `self._replace` and `ModelObject.replace_with_*`, to expose APIs of `ModelObject`s and allows manipulation and rendering without `Scene`.
 2. Expose `create_capsule` and `create_cube` APIs.
+
+## 0.3.0
+
+1. Fix `gl_FrontFacing` computation in pipeline so it is consistent to comment: `True` if not backfacing (i.e. frontfacing & side facing).
+2. Add an extra stage `Shader.primitive_chooser` to choose which primitive to be rendered for each fragment. The default implementation is provided, which assumes that the depth is just the interpolated `z` value in the eye space. It just picks the values of the single primitive that is closest to the camera and is not discarded in the previous pipeline.
+3. Expose `loop_unroll` static option to allow unrolling several operations (row rendering) within a single iteration of the outmost loop (iterating along first axis of the canvas). This may be useful in some cases for performance improvement, but careful benchmarking is needed to determine the optimal value. The default value is `1` (no unrolling) as it is the most general case in larger canvases (benchmarked on `960x540` using [GPU T4 in Colab](https://colab.research.google.com/drive/1xhkYNz5WjvUCjQWpp72CLf9SIy3i5PnN)).
+4. Bump the minimum Python version to Python 3.10
+5. Lower the minimum jax & jaxlib version to 0.3.25.
```

### Comparing `jaxrenderer-0.2.1/pyproject.toml` & `jaxrenderer-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaxrenderer"
-version = "0.2.1"
+version = "0.3.0"
 description = "Jax implementation of rasterizer renderer."
 authors = ["Joey Teng <joey.teng.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JoeyTeng/jaxrenderer"
 repository = "https://github.com/JoeyTeng/jaxrenderer"
 classifiers = [
@@ -28,18 +28,18 @@
     "README.md",
     "changelog.md",
     "pyproject.toml",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
-jax = "^0.4.4"
+python = "^3.10"
+jax = ">=0.3.25,<5.0.0"
 numpy = "^1.22.0"
-jaxlib = {version = "^0.4.4", source = "jax"}
+jaxlib = {version = ">=0.3.25,<5.0.0", source = "jax"}
 jaxtyping = "^0.2.19"
 importlib-metadata = "^6.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.6.2"
 pillow = "^9.4.0"
```

### Comparing `jaxrenderer-0.2.1/renderer/README.md` & `jaxrenderer-0.3.0/renderer/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,18 +33,26 @@
 
 Implemented in pipeline and cannot be changed.
 
 The fragments are generated for each position in the zbuffer, and if the screen coordinate is in one primitive, the relevant fragment is passed to the fragment shader for computation.
 
 The processing is done by iterating along the first axis of the buffer, and `vmap` along the second axis, and `vmap` along the primitives. Thus, all fragments at the same position are generated together, then mixed, then written to the buffer.
 
-Interpolation of all attributes for each fragment is defined by `Shader.interpolate`. The default implementation is provided, which simply linearly interpolates the attributes in the clip space according to the barycentric coordinates of the fragment. This behaviour is wrapped as a convenient function `interpolate` and mode `Interpolation.SMOOTH`. The interpolated values are then passed to the fragment shader.
-
 Currently no anti-aliasing strategy is supported.
 
+#### Optional Early Depth Test
+
+This is an additional stage in this pipeline which may be analogical to the early depth test in OpenGL. It is implemented in `Shader.primitive_chooser`. The default implementation is provided, which assumes that the depth is just the interpolated `z` value in the eye space. It just picks the values of the single primitive that is closest to the camera and is not discarded in the previous pipeline.
+
+Custom implementations can overload to change this behaviour to achieve special effects like occlusion, transparency, etc. Note that the number of returned primitives must be static, i.e., same for all fragments, as required by `jax.jit`.
+
+#### Interpolation of Attributes
+
+Interpolation of all attributes for each fragment is defined by `Shader.interpolate`. The default implementation is provided, which simply linearly interpolates the attributes in the clip space according to the barycentric coordinates of the fragment. This behaviour is wrapped as a convenient function `interpolate` and mode `Interpolation.SMOOTH`. The interpolated values are then passed to the fragment shader. Currently only `Interpolation.SMOOTH` and `Interpolation.FLAT` are supported.
+
 Reference:
 
 - For interpolation modes, see [Interpolation Qualifiers](https://www.khronos.org/opengl/wiki/Type_Qualifier_(GLSL)#Interpolation_qualifiers)
 
 ### Fragment Processing
 
 This is done by `Shader.fragment`. A default implementation is provided, which simply returns the `z` component of the fragment position in the screen space as the depth, and directly returns all extra attributes.
```

### Comparing `jaxrenderer-0.2.1/renderer/__init__.py` & `jaxrenderer-0.3.0/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.1/renderer/geometry.py` & `jaxrenderer-0.3.0/renderer/geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, NamedTuple, Optional, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Float, Integer, Num, jaxtyped
 
+from ._meta_utils import add_tracing_name
 from .types import Triangle2Df, Vec2f, Vec3f, Vec4f
 
 # Transform matrix that takes a batch of homogeneous 3D vertices and transform
 # them into 2D cartesian vertices in screen space + Z value (making it 3D)
 #
 # The result of x-y values in screen space may be float, and thus further
 # conversion to integers are needed.
@@ -24,15 +25,16 @@
 # Transform all coordinates from clip space in a bi-unit cube ([-1...1]^3) to
 # a screen cube ([x, x+width] * [y, y+height] * [0, depth]) in view space.
 # (Normalised Device Coordinates -> Window Coordinates)
 Viewport = Float[Array, "4 4"]
 
 
 @jaxtyped
-@partial(jax.jit, donate_argnums=(0, ))
+@partial(jax.jit, donate_argnums=(0, ), inline=True)
+@add_tracing_name
 def normalise(vector: Float[Array, "dim"]) -> Float[Array, "dim"]:
     """normalise vector in-place."""
     return vector / jnp.linalg.norm(vector)
 
 
 class Interpolation(enum.Enum):
     """Interpolation methods for rasterisation.
@@ -44,15 +46,16 @@
     """Flat shading: use the value of the first vertex of the primitive""" ""
     NOPERSPECTIVE = 1
     """No perspective correction: linear interpolation in screen space"""
     SMOOTH = 2
     """Perspective correction: linear interpolation in clip space"""
 
     @jaxtyped
-    @partial(jax.jit, static_argnames=("self", ))
+    @partial(jax.jit, static_argnames=("self", ), inline=True)
+    @add_tracing_name
     def __call__(
         self,
         values: Num[Array, "3 *valueDimensions"],
         barycentric_screen: Vec3f,
         barycentric_clip: Vec3f,
     ) -> Num[Array, "*valueDimensions"]:
         """Interpolation, using barycentric coordinates.
@@ -88,15 +91,16 @@
             (((0, ), (0, )), ([], [])),
         )
 
         return interpolated
 
 
 @jaxtyped
-@partial(jax.jit, static_argnames=("mode", ))
+@partial(jax.jit, static_argnames=("mode", ), inline=True)
+@add_tracing_name
 def interpolate(
     values: Num[Array, "3 *valueDimensions"],
     barycentric_screen: Vec3f,
     barycentric_clip: Vec3f,
     mode: Interpolation = Interpolation.SMOOTH,
 ) -> Num[Array, "*valueDimensions"]:
     """Convenient wrapper, see `Interpolation.__call__`.
@@ -111,15 +115,16 @@
     )
     assert isinstance(interpolated, Num[Array, "*valueDimensions"])
 
     return interpolated
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def to_homogeneous(
     coordinates: Float[Array, "*batch dim"],
     value: Float[Array, "*batch"] = jnp.array(1.),
 ) -> Float[Array, "*batch dim+1"]:
     """Transform the coordinates to homogeneous coordinates by append a batch
         of `value`s (default 1.) in the last axis."""
     if not isinstance(value, Float[Array, "*batch"]):
@@ -134,29 +139,31 @@
         jnp.ndim(coordinates) - 1,
     )
 
     return homo_coords
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def normalise_homogeneous(
     coordinates: Float[Array, "*batch dim"], ) -> Float[Array, "*batch dim"]:
     """Transform the homogenous coordinates to make the scale factor equals to
         either 1 or 0, by divide every element with the last element on the
         last axis.
 
     Noted that when a coordinate is 0 and divides by 0, it will produce a nan;
     for non-zero elements divides by 0, a inf will be produced.
     """
     return coordinates / coordinates[..., -1:]
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def to_cartesian(
     coordinates: Float[Array, "*batch dim"], ) -> Float[Array, "*batch dim-1"]:
     """Transform the homogenous coordinates to cartesian coordinates by divide
         every element with the last element on the last axis, then drop them.
 
     When last component is 0, this function just discard the w-component
     without division.
@@ -188,15 +195,16 @@
     world_to_eye_norm: Projection
     world_to_screen: World2Screen
     view_inv: View
     screen_to_world: World2Screen
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ))
+    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @add_tracing_name
     def create(
         cls,
         view: View,
         projection: Projection,
         viewport: Viewport,
         view_inv: Optional[View] = None,
     ) -> "Camera":
@@ -236,15 +244,16 @@
             world_to_screen=viewport @ projection @ view,
             view_inv=view_inv,
             screen_to_world=view_inv @ projection_inv @ viewport_inv,
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def apply(
         points: Num[Array, "*N 4"],
         matrix: Num[Array, "4 4"],
     ) -> Num[Array, "*N 4"]:
         """Transform homogeneous points using given matrix.
 
         Parameters:
@@ -271,15 +280,16 @@
         )
         assert isinstance(transformed, Num[Array, "*N 4"])
 
         return transformed
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ))
+    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @add_tracing_name
     def apply_pos(
         cls,
         points: Num[Array, "*N 3"],
         matrix: Num[Array, "4 4"],
     ) -> Num[Array, "*N 3"]:
         """Transform points representing 3D positions using given matrix.
 
@@ -301,15 +311,16 @@
         transformed = to_cartesian(transformed_homo)
         assert isinstance(transformed, Num[Array, "*N 3"])
 
         return transformed
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ))
+    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @add_tracing_name
     def apply_vec(
         cls,
         vectors: Num[Array, "*N 3"],
         matrix: Num[Array, "4 4"],
     ) -> Num[Array, "*N 3"]:
         """Transform vectors representing 3D positions using given matrix.
 
@@ -339,15 +350,16 @@
 
         transformed_normalised = normalise(transformed)
         assert isinstance(transformed_normalised, Num[Array, "*N 3"])
 
         return transformed_normalised
 
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def to_screen(
         self,
         points: Num[Array, "*N 4"],
     ) -> Num[Array, "*N 4"]:
         """Transform points from model space to screen space.
 
         Parameters:
@@ -364,15 +376,16 @@
 
         normalised = normalise_homogeneous(screen_space)
         assert isinstance(normalised, Num[Array, "*N 4"])
 
         return normalised
 
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def to_clip(
         self,
         points: Num[Array, "*N 4"],
     ) -> Num[Array, "*N 4"]:
         """Transform points from model space to screen space.
 
         Parameters:
@@ -386,15 +399,16 @@
         """
         clip_space = self.apply(points, self.world_to_clip)
         assert isinstance(clip_space, Num[Array, "*N 4"])
 
         return clip_space
 
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def to_screen_inv(
         self,
         screen: Float[Array, "*N 4"],
     ) -> Float[Array, "*N 4"]:
         """Transform points from screen space to model space.
 
         This is an inverse process of `to_screen`, and provide higher precision
@@ -438,15 +452,16 @@
             normalise_homogeneous(world),
         )
 
         return world
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def inv_scale_translation_matrix(
             scale_translation_mat: Float[Array, "4 4"]) -> Float[Array, "4 4"]:
         """Compute the inverse matrix of a (4, 4) matrix representing a scale and translation, in a form of:
 
             [[s_x, 0,   0,   t_x],
              [0,   s_y, 0,   t_y],
              [0,   0,   s_z, t_z],
@@ -479,15 +494,16 @@
         scale_translation_inv = translation_inv @ scale_inv
         assert isinstance(scale_translation_inv, Float[Array, "4 4"])
 
         return scale_translation_inv
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def view_matrix(
         eye: Vec3f,
         centre: Vec3f,
         up: Vec3f,
     ) -> View:
         """Compute View matrix as defined by OpenGL / tinyrenderer.
 
@@ -520,15 +536,16 @@
 
         view: View = m @ translation
 
         return view
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def view_matrix_inv(
         eye: Vec3f,
         centre: Vec3f,
         up: Vec3f,
     ) -> View:
         """Compute the invert of View matrix as defined by OpenGL.
 
@@ -573,15 +590,16 @@
         view_matrix_inv: View = translation_inv @ m_inv
         assert isinstance(view_matrix_inv, View)
 
         return view_matrix_inv
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def perspective_projection_matrix(
         fovy: jnp.floating[Any],
         aspect: jnp.floating[Any],
         z_near: jnp.floating[Any],
         z_far: jnp.floating[Any],
     ) -> Projection:
         """Create a projection matrix to map the model in the camera frame (eye
@@ -617,15 +635,16 @@
             .at[3, 2].set(-1.)  # let \omega be -z
         )
 
         return projection
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ))
+    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @add_tracing_name
     def perspective_projection_matrix_inv(cls, mat: Projection) -> Projection:
         """Create the inverse of a perspective projection matrix as defined in
             `perspective_projection_matrix`.
 
         Since the perspective projection matrix is formed as:
 
             [[a, 0,  0, 0],
@@ -646,15 +665,16 @@
         inv = cls.inv_scale_translation_matrix(mat[:, shuffle])[shuffle, :]
         assert isinstance(inv, Projection)
 
         return inv
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def orthographic_projection_matrix(
         left: jnp.floating[Any],
         right: jnp.floating[Any],
         bottom: jnp.floating[Any],
         top: jnp.floating[Any],
         z_near: jnp.floating[Any],
         z_far: jnp.floating[Any],
@@ -690,28 +710,30 @@
         )
 
         return projection
 
     @classmethod
     @jaxtyped
     @partial(jax.jit, static_argnames=("cls", ))
+    @add_tracing_name
     def orthographic_projection_matrix_inv(cls, mat: Projection) -> Projection:
         """Create the inverse of a orthographic projection matrix as defined in
             `orthographic_projection_matrix`. Since orthographic projection
             matrix is a scale-translation matrix, the inverse is computed by
             `inv_scale_translation_matrix` directly.
         """
         inv = cls.inv_scale_translation_matrix(mat)
         assert isinstance(inv, Projection)
 
         return inv
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def perspective_projection_matrix_tinyrenderer(
         eye: Vec3f,
         centre: Vec3f,
         dtype: jnp.dtype = jnp.single,
     ) -> Projection:
         """Create a projection matrix to map the model in the camera frame (eye
             coordinates) onto the viewing volume (clip coordinates), using
@@ -730,15 +752,16 @@
             .at[3, 2].set(-1 / jnp.linalg.norm(eye - centre))  #
         )
 
         return projection
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def viewport_matrix(
         lowerbound: Num[Array, "2"],
         dimension: Integer[Array, "2"],
         depth: Num[Array, ""],
     ) -> Viewport:
         """Create a viewport matrix to map the model in bi-unit cube
             ([-1...1]^3) onto the screen cube ([x, x+w]*[y, y+h]*[0, d]). The
@@ -762,15 +785,16 @@
             .at[2, 2:].set(depth / 2)  #
         )
 
         return viewport
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ))
+    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @add_tracing_name
     def viewport_matrix_inv(cls, viewport: Viewport) -> Viewport:
         """Create the inverse of a viewport matrix as defined in `viewport_matrix`.
 
         Parameters:
           - viewport: Viewport matrix to invert.
 
         Return: Viewport^{-1}, (4, 4) matrix.
@@ -778,15 +802,16 @@
         viewport_inv: Viewport = cls.inv_scale_translation_matrix(viewport)
         assert isinstance(viewport_inv, Viewport)
 
         return viewport_inv
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def world_to_screen_matrix(width: int, height: int) -> World2Screen:
         """Generate the projection matrix to convert model coordinates to
             screen/canvas coordinates.
 
         It assumes all model coordinates are in [-1...1] and will transform them
         into ([0...width], [0...height], [-1...1]).
 
@@ -800,34 +825,37 @@
             # 1. Add by 1 to make values positive
             @ jnp.identity(4).at[:2, -1].set(1))
 
         return world2screen
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def compute_normal(triangle_verts: Float[Array, "3 3"]) -> Float[Array, "3"]:
     normal: Float[Array, "3"] = jnp.cross(
         triangle_verts[2, :] - triangle_verts[0, :],
         triangle_verts[1, :] - triangle_verts[0, :],
     )
     normal = normal / jnp.linalg.norm(normal, keepdims=True)
     assert isinstance(normal, Float[Array, "3"])
 
     return normal
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def compute_normals(batch_verts: Float[Array, "b 3 3"]) -> Float[Array, "b 3"]:
     return jax.vmap(compute_normal)(batch_verts)
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def quaternion(
     rotation_axis: Union[Vec3f, tuple[float, float, float]],
     rotation_angle: Union[Float[Array, ""], float],
 ) -> Vec4f:
     """Generate a quaternion rotation from a rotation axis and angle.
 
     The rotation axis is normalised internally. The angle is specified in
@@ -846,15 +874,16 @@
         .at[1:].set(axis * jnp.sin(angle / 2))  #
     )
 
     return quaternion
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def quaternion_mul(quatA: Vec4f, quatB: Vec4f) -> Vec4f:
     """Multiply two quaternion rotations, as to composite them.
 
     Noticed that all quaternions here are in order of (w, x, y, z).
 
     References:
       - [Quaternion multiplication](https://www.mathworks.com/help/nav/ref/quaternion.mtimes.html)
@@ -873,15 +902,16 @@
         quatA[:3] @ quatB[idx103] - quatA[3] * quatB[2],
         quatA[idx230] @ quatB[:3] - quatA[1] * quatB[3],
         quatA[idx013] @ quatB[idx320] - quatA[2] * quatB[1],
     ))
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def rotation_matrix(
     rotation_axis: Union[Vec3f, tuple[float, float, float]],
     rotation_angle: Union[Float[Array, ""], float],
 ) -> Float[Array, "3 3"]:
     """Generate a rotation matrix from a rotation axis and angle.
 
     The rotation axis is normalised internally. The angle is specified in
@@ -904,15 +934,16 @@
         + (1 - c) * jnp.outer(axis, axis)  # first term
     )
 
     return rotation_matrix
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def transform_matrix_from_rotation(rotation: Vec4f) -> Float[Array, "3 3"]:
     """Generate a transform matrix from a quaternion rotation.
 
     Quaternion is specified in (w, x, y, z) order. Supports non-unit rotation.
 
     References:
           - [Quaternions and spatial rotation#Quaternion-derived rotation matrix](https://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation#Quaternion-derived_rotation_matrix)
@@ -932,15 +963,16 @@
     ))
     assert isinstance(mat, Float[Array, "3 3"])
 
     return mat
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def barycentric(pts: Triangle2Df, p: Vec2f) -> Vec3f:
     """Compute the barycentric coordinate of `p`.
         Returns u[-1] < 0 if `p` is outside of the triangle.
     """
     mat: Float[Array, "3 2"] = jnp.vstack((
         pts[2] - pts[0],
         pts[1] - pts[0],
```

### Comparing `jaxrenderer-0.2.1/renderer/model.py` & `jaxrenderer-0.3.0/renderer/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import jax.experimental.checkify as checkify
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import tree_map
 from jaxtyping import (Array, Bool, Float, Integer, Num, PyTree, Shaped,
                        jaxtyped)
 
+from ._meta_utils import add_tracing_name
 from .geometry import Camera, transform_matrix_from_rotation
 from .types import (FALSE_ARRAY, FaceIndices, Normals, SpecularMap, Texture,
                     UVCoordinates, Vec3f, Vec4f, Vertices)
 from .value_checker import index_in_bound
 
 ModelMatrix = Float[Array, "4 4"]
 
@@ -158,14 +159,15 @@
     offset: Integer[Array, ""]
     """Width of biggest merged maps, as [0] returned by `merge_maps`."""
     diffuse_map: Texture
     specular_map: SpecularMap
 
     @staticmethod
     @jaxtyped
+    @add_tracing_name
     def generate_object_vert_info(
         counts: Sequence[int],
         values: Sequence[Shaped[Array, "..."]],
     ) -> Shaped[Array, "vertices"]:
         """Generate object-wide info for each vertex in merged model as
             vertex-level info.
 
@@ -187,15 +189,16 @@
         )
         map_indices = lax.concatenate(values, dimension=0)
 
         return map_indices
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def merge_verts(
         vs: VertsT,
         fs: FaceIndicessT,
     ) -> tuple[VertT, FaceIndicesT]:
         """"""
         counts = [v.shape[0] for v in vs[:-1]]
         cumsum = [0]
@@ -215,15 +218,16 @@
             dimension=0,
         )
 
         return verts, faces
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def merge_maps(maps: MapsT) -> tuple[MapT, Shape2DT]:
         """Merge maps by concatenating them along the first axis.
 
         All maps must have the same number of dimensions, i.e., `len(m.shape)`
         must be the same for all maps `m`.
 
         If the other axises is not the same, they are padded with undefined
@@ -265,15 +269,16 @@
             dimension=0,
         )
 
         return new_map, single_shape[:2]
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def uv_repeat(
         uv: Float[Array, "2"],
         shape: Integer[Array, "2"],
         map_index: Integer[Array, ""],
         offset: Integer[Array, ""],
     ) -> Float[Array, "2"]:
         """Compute final UV coordinates as if it is repeatedly tiled (in case
@@ -386,27 +391,29 @@
 
         Parameters:
           - double_sided: whether the object is double-sided.
         """
         return self._replace(double_sided=double_sided)
 
 
+@add_tracing_name
 def batch_models(models: Sequence[MergedModel]) -> MergedModel:
     """Merge multiple MergedModel into one, with each field being a batch, with
         batch axis at 0. This is intended to facilitate `jax.vmap`.
     """
     merged_model = MergedModel._make((lax.concatenate(
         [jnp.asarray(model[i])[None, ...] for model in models],
         dimension=0,
     ) for i in range(len(models[0]))))
 
     return merged_model
 
 
 @jaxtyped
+@add_tracing_name
 def merge_objects(objects: Sequence[ModelObject]) -> MergedModel:
     """Merge objects into a single model.
 
     Parameters:
       - objects: a list of objects to merge.
 
     Returns: A model containing the merged objects into one single mesh.
@@ -438,14 +445,15 @@
     # merge maps
     diffuse_map, single_map_shape = MergedModel.merge_maps(
         [m.diffuse_map for m in models])
     specular_map, _ = MergedModel.merge_maps([m.specular_map for m in models])
 
     @jaxtyped
     @partial(jax.jit, inline=True)
+    @add_tracing_name
     def transform_vert(
         verts: Float[Array, "N 3"],
         local_scaling: Vec3f,
         transform: ModelMatrix,
     ) -> Vertices:
         """Apply transforms defined in `ModelObject` to vertices."""
         world: Float[Array, "N 3"] = Camera.apply_pos(
@@ -466,14 +474,15 @@
             ) for obj in objects
         ],
         [m.faces for m in models],
     )
 
     @jaxtyped
     @partial(jax.jit, inline=True)
+    @add_tracing_name
     def transform_normals(
         normals: Float[Array, "N 3"],
         transform: ModelMatrix,
     ) -> Vertices:
         """Apply transforms defined in `ModelObject` to vertex normals."""
         world: Float[Array, "N 3"] = Camera.apply_vec(
             normals,
```

### Comparing `jaxrenderer-0.2.1/renderer/pipeline.py` & `jaxrenderer-0.3.0/renderer/pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from functools import partial
-from typing import Any, NamedTuple, TypeVar
+from typing import Any, NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax import lax
 from jax.tree_util import tree_map
 from jaxtyping import Array, Bool, Float, Integer, Num, jaxtyped
 
+from ._meta_utils import add_tracing_name
 from .geometry import Camera, Interpolation, Viewport, interpolate
 from .shader import (ID, MixedExtraT, MixerOutput, PerFragment, PerVertex,
                      Shader, ShaderExtraInputT, VaryingT)
-from .types import (FALSE_ARRAY, Buffers, FaceIndices, Triangle, Vec2f, Vec2i,
-                    Vec3f, Vec4f)
+from .types import (FALSE_ARRAY, Buffers, CanvasMask, FaceIndices, Triangle,
+                    Vec2f, Vec2i, Vec3f, Vec4f, ZBuffer)
 
 jax.config.update('jax_array', True)
 
+RowIndices = Integer[Array, "row_batches row_batch_size"]
+"""Indices of the rows in the buffers to be processed in this batch."""
+
 
 class PerPrimitive(NamedTuple):
     """Input for each primitive, using outputs from Vertex Shader.
 
     gl_Position is in clip-space, not normalised.
     """
     gl_Position: Triangle
@@ -41,15 +45,16 @@
         When determinant is 0, the triangle will not be rendered for now.
     """
     matrix_inv: Float[Array, "3 3"]
     """inverse of the matrix described above (of [x, y, w])."""
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ))
+    @partial(jax.jit, static_argnames=("cls", ), inline=True)
+    @add_tracing_name
     def create(cls, per_vertex: PerVertex) -> "PerPrimitive":
         """per_vertex is batched with size 3 (3 vertices per triangle)
             in clip-space, not normalised.
         """
         clip: Triangle = per_vertex.gl_Position
         assert isinstance(clip, Triangle)
         # matrix with x, y, w
@@ -59,62 +64,80 @@
         # `jnp.linalg.det` has built-in 3x3 det optimisation
         determinant: Float[Array, ""] = jnp.linalg.det(matrix)
         assert isinstance(determinant, Float[Array, ""])
 
         # an arbitrary number for numerical stability
         keep: Bool[Array, ""] = lax.abs(determinant) > 1e-6
 
-        mat_inv: Float[Array, "3 3"] = lax.cond(
-            # an arbitrary number for numerical stability
-            keep,
-            # may replace with custom implementation for higher precision
-            lambda: jnp.linalg.inv(matrix),
-            lambda: jnp.zeros((3, 3)),
-        )
+        # although this may result in NaN or Inf when keep is False,
+        # it will be discarded later.
+        # Perf: Remove lax.cond to reduce extra operations `select_n` in HLO.
+        mat_inv: Float[Array, "3 3"] = jnp.linalg.inv(matrix)
         assert isinstance(mat_inv, Float[Array, "3 3"])
 
         return cls(
             gl_Position=clip,
             keep=keep,
             determinant=determinant,
             matrix_inv=mat_inv,
         )
 
 
 @jaxtyped
-@partial(jax.jit, static_argnames=("shader", ), donate_argnums=(1, ))
+@partial(
+    jax.jit,
+    static_argnames=("shader", "loop_unroll"),
+    donate_argnums=(1, ),
+    inline=True,
+)
+@add_tracing_name
 def _postprocessing(
     shader: type[Shader[ShaderExtraInputT, VaryingT, MixedExtraT]],
     buffers: Buffers,
     per_primitive: tuple[Any, ...],  # Batch PerPrimitive
     varyings: VaryingT,
     extra: ShaderExtraInputT,
     viewport: Viewport,
+    loop_unroll: int,
 ) -> Buffers:
     with jax.ensure_compile_time_eval():
-        # loop along first axis, for memory efficiency
-        # TODO: benchmark if this is actually faster
-        loop_size: int = int(buffers[0].shape[0])
         # vmap batch along second axis
         batch_size: int = int(buffers[0].shape[1])
+        row_indices: Integer[Array, "width"]
+        row_indices = lax.iota(int, int(buffers[0].shape[0]))
 
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def _per_pixel(coord: Vec2i) -> tuple[MixerOutput, MixedExtraT]:
 
         assert isinstance(coord, Vec2i), f"expected Vec2i, got {coord}"
 
+        ReturnT = tuple[  #
+            Float[Array, "kept_primitives 4"],  #
+            Bool[Array, "kept_primitives"],  #
+            Float[Array, "kept_primitives 2"],  #
+            Bool[Array, "kept_primitives"],  #
+            VaryingT,  #
+            Float[Array, "kept_primitives 3"],  #
+            Float[Array, "kept_primitives 3"],  #
+        ]
+
         @jaxtyped
-        def _per_primitive_process(
+        @partial(jax.jit, inline=True)
+        @add_tracing_name
+        def _per_primitive_preprocess(
             primitive: PerPrimitive,
             varying_per_primitive: VaryingT,
-        ) -> tuple[PerFragment, VaryingT]:
-            # PROCESS: Interpolation
+        ) -> ReturnT:
+            # PROCESS: Early Culling (`primitive_chooser`)
 
             # For early exit when not keep primitive / determinant is 0
+            @partial(jax.jit, inline=True)
+            @add_tracing_name
             def _when_keep_primitive() -> tuple[Vec3f, Float[Array, ""]]:
                 """Returns clip_coef, w_reciprocal."""
                 # x/w, y/w, with x, y, w in clip space.
                 xy: Float[Array, "2"] = (
                     (coord - viewport[:2, 3]) /
                     viewport[jnp.arange(2), jnp.arange(2)])
                 xy1_ndc: Float[Array, "3"] = jnp.array((xy[0], xy[1], 1))
@@ -132,24 +155,25 @@
                 w_reciprocal: Float[Array, ""] = clip_coef.sum()
                 assert isinstance(w_reciprocal, Float[Array, ""])
 
                 return clip_coef, w_reciprocal
 
             # END OF `_when_keep_primitive`
 
-            # Prepare for interpolation parameters
-            # clip_coef here interpolates to 1/w * target value
-            clip_coef, w_reciprocal = lax.cond(
-                # an arbitrary number for numerical stability
-                primitive.keep,
-                _when_keep_primitive,
-                lambda: (lax.full((3, ), -1.), jnp.zeros(())),
-            )
-
-            def _when_in_triangle() -> tuple[PerFragment, VaryingT]:
+            @partial(jax.jit, inline=True)
+            @add_tracing_name
+            def _when_in_triangle(
+                clip_coef: Vec3f,
+                w_reciprocal: Float[Array, ""],
+            ) -> tuple[  #
+                    Float[Array, "kept_primitives 4"],  # gl_FragCoord
+                    Bool[Array, "kept_primitives"],  # gl_FrontFacing
+                    Float[Array, "kept_primitives 2"],  # gl_PointCoord
+                    Float[Array, "kept_primitives 3"],  # true_clip_coef
+            ]:
                 # Prepare inputs for fragment shader
                 z: Float[Array, ""] = interpolate(
                     values=primitive.gl_Position[:, 2],
                     barycentric_screen=clip_coef,
                     barycentric_clip=clip_coef,
                     mode=Interpolation.SMOOTH,
                 )
@@ -160,198 +184,264 @@
                     coord[1],
                     z,
                     w_reciprocal,
                 ))
                 assert isinstance(gl_FragCoord, Vec4f)
 
                 # Ref: https://registry.khronos.org/OpenGL-Refpages/gl4/html/gl_FrontFacing.xhtml
-                gl_FrontFacing: Bool[Array, ""] = primitive.determinant > 0
+                # True if not back-facing.
+                gl_FrontFacing: Bool[Array, ""] = primitive.determinant >= 0
                 assert isinstance(gl_FrontFacing, Bool[Array, ""])
 
                 gl_PointCoord: Vec2f
                 with jax.ensure_compile_time_eval():
                     # TODO: implement Point primitive properly.
-                    gl_PointCoord = lax.full((2, ), 0)
+                    gl_PointCoord = lax.full((2, ), 0.)
 
                 # this interpolates to target value u, not u/w
                 true_clip_coef: Vec3f = clip_coef / w_reciprocal
                 assert isinstance(true_clip_coef, Vec3f)
 
-                varying: VaryingT = shader.interpolate(
-                    values=varying_per_primitive,
-                    barycentric_screen=true_clip_coef,
-                    barycentric_clip=true_clip_coef,
-                )
-                assert isinstance(varying, tuple)
-
-                # PROCESS: Fragment Processing
-                per_frag: PerFragment
-                extra_fragment_output: VaryingT
-                per_frag, extra_fragment_output = shader.fragment(
-                    gl_FragCoord=gl_FragCoord,
-                    gl_FrontFacing=gl_FrontFacing,
-                    gl_PointCoord=gl_PointCoord,
-                    varying=varying,
-                    extra=extra,
-                )
-                assert isinstance(per_frag, PerFragment)
-                assert isinstance(extra_fragment_output, tuple)
-
-                # enforce default `gl_FragDepth` when it is None
-                per_frag = lax.cond(
-                    per_frag.use_default_depth,
-                    lambda: per_frag._replace(gl_FragDepth=gl_FragCoord[2]),
-                    lambda: per_frag,
-                )
-                assert isinstance(per_frag, PerFragment)
-
-                return per_frag, extra_fragment_output
+                return (gl_FragCoord, gl_FrontFacing, gl_PointCoord,
+                        true_clip_coef)
 
             # END OF `_when_in_triangle`
 
+            # Prepare for interpolation parameters
+            # clip_coef here interpolates to 1/w * target value
+            # Perf: although this may result in garbage values (NaN or Inf)
+            # when keep is False, since it will be discarded later, we can
+            # remove the lax.cond to reduce extra operations `select_n` in HLO
+            # as the computation is quite cheap.
+            # also see google/brax#8409 for why `_when_keep_primitive` is
+            # always executed.
+            clip_coef, w_reciprocal = _when_keep_primitive()
+
             in_triangle: Bool[Array, ""] = (clip_coef >= 0).all()
             assert isinstance(in_triangle, Bool[Array, ""])
 
-            built_in: PerFragment
-            attachments: VaryingT
-            built_in, attachments = lax.cond(
-                jnp.logical_and(primitive.keep, in_triangle),
-                _when_in_triangle,
-                # discard out-of-triangle values
-                lambda: (
-                    PerFragment(keeps=FALSE_ARRAY),
-                    # dummy values
-                    tree_map(lambda field: field[0], varying_per_primitive),
-                ),
+            # Perf: although this may result in garbage values (NaN or Inf)
+            # when keep or in_triangle is False, since it will be discarded
+            # later, we can remove the lax.cond to reduce extra operations
+            # `select_n` in HLO.
+            # See google/brax#8409 for why `_when_keep_primitive` is always
+            # executed.
+            # TODO: change back to `lax.cond` when it does not force execute both branches under vmap.
+            r = _when_in_triangle(clip_coef, w_reciprocal)
+            gl_FragCoord, gl_FrontFacing, gl_PointCoord, true_clip_coef = r
+
+            return (
+                gl_FragCoord,
+                gl_FrontFacing,
+                gl_PointCoord,
+                primitive.keep & in_triangle,
+                varying_per_primitive,
+                true_clip_coef,
+                true_clip_coef,
+            )
+
+        # END OF `_per_primitive_preprocess`
+
+        @partial(jax.jit, inline=True)
+        @add_tracing_name
+        def _interpolate_and_fragment_shading(
+            gl_FragCoord: Vec4f,
+            gl_FrontFacing: Bool[Array, ""],
+            gl_PointCoord: Vec2f,
+            keeps: Bool[Array, ""],
+            values: VaryingT,
+            barycentric_screen: Vec3f,
+            barycentric_clip: Vec3f,
+        ) -> tuple[PerFragment, VaryingT]:
+            # PROCESS: Interpolation
+            varying: VaryingT = shader.interpolate(
+                values=values,
+                barycentric_screen=barycentric_screen,
+                barycentric_clip=barycentric_clip,
+            )
+            assert isinstance(varying, tuple)
+
+            # PROCESS: Fragment Processing
+            per_frag: PerFragment
+            extra_fragment_output: VaryingT
+            per_frag, extra_fragment_output = shader.fragment(
+                gl_FragCoord=gl_FragCoord,
+                gl_FrontFacing=gl_FrontFacing,
+                gl_PointCoord=gl_PointCoord,
+                varying=varying,
+                extra=extra,
             )
-            assert isinstance(built_in, PerFragment)
-            assert isinstance(attachments, tuple)
+            assert isinstance(per_frag, PerFragment)
+            assert isinstance(extra_fragment_output, tuple)
+
+            # enforce default `gl_FragDepth` when `use_default_depth`
+            per_frag = lax.cond(
+                per_frag.use_default_depth,
+                lambda: per_frag._replace(gl_FragDepth=gl_FragCoord[2]),
+                lambda: per_frag,
+            )
+            assert isinstance(per_frag, PerFragment)
+
+            per_frag = per_frag._replace(keeps=keeps & per_frag.keeps)
 
-            return built_in, attachments
+            return per_frag, extra_fragment_output
 
-        # END OF `_per_primitive_process`
+        # END OF `_interpolate_fragment_shading`
 
-        built_in, extra_outputs = jax.vmap(_per_primitive_process)(
+        args = jax.vmap(_per_primitive_preprocess)(
             per_primitive,
             varyings,
         )
+        chosen_args = shader.primitive_chooser(*args)
+
+        built_in: PerFragment
+        extra_outputs: VaryingT
+        _f = jax.vmap(_interpolate_and_fragment_shading)
+        built_in, extra_outputs = _f(*chosen_args)
+        assert isinstance(built_in, PerFragment)
+
         gl_Depths = built_in.gl_FragDepth
         keeps = built_in.keeps
+        assert isinstance(gl_Depths, Float[Array, "kept_primitives"])
+        assert isinstance(keeps, Bool[Array, "kept_primitives"])
 
         # PROCESS: Per-Sample Operations (Mixing: depth test + colour blending)
         mixed_output: MixerOutput
         attachments: MixedExtraT
         mixed_output, attachments = shader.mix(gl_Depths, keeps, extra_outputs)
         assert isinstance(mixed_output, MixerOutput)
         assert isinstance(attachments, tuple)
 
         return mixed_output, attachments
 
-    @jaxtyped
-    @partial(jax.jit, donate_argnums=(1, ))
-    def loop_body(
-        index: Integer[Array, ""],
-        buffers: Buffers,
-    ) -> Buffers:
-
-        _valueT = TypeVar('_valueT', bound=tuple[Any, ...])
-
-        @jaxtyped
-        @partial(jax.jit, donate_argnums=(2, ))
-        def select_value_per_pixel(
-            keep: Bool[Array, ""],
-            new_values: _valueT,
-            old_values: _valueT,
-        ) -> _valueT:
-            """Choose new value of the pixel, or keep the previous."""
-            FieldRowT = TypeVar("FieldRowT")
-
-            def _select_per_field(
-                new_field_value: FieldRowT,
-                old_field_value: FieldRowT,
-            ) -> FieldRowT:
-                """Choose this pixel for this field in the PyTree."""
-                return lax.cond(
-                    keep,
-                    lambda: new_field_value,
-                    lambda: old_field_value,
-                )
-
-            # tree_map over each field in the PyTree
-            result: _valueT = tree_map(
-                _select_per_field,
-                new_values,
-                old_values,
-            )
+    # END OF `_per_pixel`
 
-            return result
+    @jaxtyped
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
+    def _per_row(i: Integer[Array, ""], ) -> tuple[MixerOutput, MixedExtraT]:
+        """Render one row.
+
+        Parameters:
+          - i: the index of the row to be rendered on the first axis of the
+            resultant buffer.
 
+        Returns: one row from `Shader.mixer`, `MixerOutput` and `MixerExtraT`.
+        """
         keeps: Bool[Array, "height"]
         depths: Num[Array, "height"]
         extras: MixedExtraT
-        # vmap over axis 1 (height) of the buffers. Axis 0 (width) is `index`.
+        # vmap over axis 1 (height) of the buffers. Axis 0 (width) is `i`.
         (keeps, depths), extras = jax.vmap(_per_pixel)(lax.concatenate(
             (
-                lax.full((batch_size, 1), index),
+                lax.full((batch_size, 1), i),
                 lax.broadcasted_iota(int, (batch_size, 1), 0),
             ),
             1,
         ))
         assert isinstance(keeps, Bool[Array, "height"])
         assert isinstance(depths, Num[Array, "height"])
         assert isinstance(extras, tuple)
 
-        # vmap each pixel over axis 1 (height) of the buffers (per row in
-        # matrix)
-        buffers_row = jax.vmap(select_value_per_pixel)(
-            keeps,
+        return MixerOutput(keep=keeps, zbuffer=depths), extras
+
+    # END OF `_per_row`
+
+    @jaxtyped
+    @partial(jax.jit, donate_argnums=(1, ), inline=True)
+    @add_tracing_name
+    def merge_buffers(
+        mixer_outputs: tuple[MixerOutput, MixedExtraT],
+        old_buffers: Buffers,
+    ) -> Buffers:
+        """Merge the rendered row into the buffers.
+
+        Parameters:
+          - mixer_outputs: the output from `Shader.mixer`, `MixerOutput` and
+            `MixerExtraT`.
+          - old_buffers: the buffers to be updated.
+
+        Returns: the updated buffers.
+        """
+        keeps: CanvasMask = mixer_outputs[0].keep
+        depths: ZBuffer = mixer_outputs[0].zbuffer
+        extras: MixedExtraT = mixer_outputs[1]
+
+        @partial(jax.jit, donate_argnums=(2, ), inline=True)
+        def _merge_first_axis(_mask, _new, _old):
+
+            @partial(jax.jit, donate_argnums=(2, ), inline=True)
+            def _merge_second_axis(__mask, __new, __old):
+                return lax.cond(__mask, lambda: __new, lambda: __old)
+
+            return jax.vmap(_merge_second_axis)(_mask, _new, _old)
+
+        new_buffers: Buffers = tree_map(
+            lambda new, old: jax.vmap(_merge_first_axis)(keeps, new, old),
             Buffers(zbuffer=depths, targets=tuple(extras)),
-            tree_map(lambda field: field[index], buffers),
+            old_buffers,
         )
+        assert isinstance(new_buffers, Buffers)
 
-        # tree_map over each field in the PyTree to update all buffers
-        return tree_map(
-            lambda field, value: field.at[index].set(value),
-            buffers,
-            buffers_row,
-        )
+        return new_buffers
 
-    # END OF `loop_body`
+    # END OF `merge_buffers`
 
-    # iterate over axis 0 (width) of the buffers (one row at a time)
-    buffers = lax.fori_loop(
-        0,
-        loop_size,
-        loop_body,
-        buffers,
-    )
+    # iterate over axis 0 (width) of the buffers
+    # (multiple row at a time, according to `row_indices``)
+    # Not using vmap due to memory constraints
+    # TODO: using map for readability when map supports unroll.
+    # Reference: https://jax.readthedocs.io/en/latest/_modules/jax/_src/lax/control_flow/loops.html#map
+    mixer_outputs = lax.scan(
+        lambda _, x: ((), _per_row(x)),
+        init=(),
+        xs=row_indices,
+        unroll=loop_unroll,
+    )[1]
+
+    buffers = merge_buffers(mixer_outputs, buffers)
     assert isinstance(buffers, Buffers)
 
     return buffers
 
 
 @jaxtyped
-@partial(jax.jit, static_argnames=("shader", ), donate_argnums=(2, ))
+@partial(
+    jax.jit,
+    static_argnames=("shader", "loop_unroll"),
+    donate_argnums=(2, ),
+    inline=True,
+)
+@add_tracing_name
 def render(
     camera: Camera,
     shader: type[Shader[ShaderExtraInputT, VaryingT, MixedExtraT]],
     buffers: Buffers,
     face_indices: FaceIndices,
     extra: ShaderExtraInputT,
+    loop_unroll: int = 1,
 ) -> Buffers:
+    """Render a scene with a shader.
+
+    Parameters:
+      - loop_unroll: the number of rows to be rendered in one loop. This may
+        help improve the performance at the cost of increasing compilation time.
+        Default: 1
+    """
     vertices_count: int
     gl_InstanceID: ID
     with jax.ensure_compile_time_eval():
         vertices_count = extra[0].shape[0]
         gl_InstanceID = jnp.array(0, dtype=int)
         assert isinstance(vertices_count, int)
         assert isinstance(gl_InstanceID, ID)
 
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def vertex_processing(
             gl_VertexID: Integer[Array, ""],  #
     ) -> tuple[PerVertex, VaryingT]:
         """Process one vertex into screen space, and keep varying values."""
         per_vertex: PerVertex
         varying: VaryingT
         per_vertex, varying = shader.vertex(
@@ -377,11 +467,12 @@
         per_primitive=jax.vmap(PerPrimitive.create)(tree_map(
             lambda field: field[face_indices],
             per_vertices,
         )),
         varyings=tree_map(lambda field: field[face_indices], varyings),
         extra=extra,
         viewport=camera.viewport,
+        loop_unroll=loop_unroll,
     )
     assert isinstance(buffers, Buffers)
 
     return buffers
```

### Comparing `jaxrenderer-0.2.1/renderer/renderer.py` & `jaxrenderer-0.3.0/renderer/renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import tree_map
 from jaxtyping import Array, Bool, Integer, Num, jaxtyped
 
+from ._meta_utils import add_tracing_name
 from .geometry import Camera, Projection, View, Viewport, normalise
 from .model import MergedModel, ModelObject, merge_objects
 from .pipeline import render
 from .shaders.phong_reflection import (PhongReflectionTextureExtraInput,
                                        PhongReflectionTextureShader)
 from .shaders.phong_reflection_shadow import (
     PhongReflectionShadowTextureExtraInput, PhongReflectionShadowTextureShader)
@@ -96,14 +97,15 @@
 
 
 class Renderer:
 
     @staticmethod
     @jaxtyped
     @partial(jax.jit, inline=True)
+    @add_tracing_name
     def create_camera_from_parameters(camera: CameraParameters) -> Camera:
         """Create a camera from camera parameters."""
         eye: Vec3f = jnp.asarray(camera.position, dtype=float)
         assert isinstance(eye, Vec3f), f"{eye}"
         centre: Vec3f = jnp.asarray(camera.target, dtype=float)
         assert isinstance(centre, Vec3f), f"{centre}"
         up: Vec3f = jnp.asarray(camera.up, dtype=float)
@@ -136,14 +138,15 @@
         )
         assert isinstance(_camera, Camera), f"{_camera}"
 
         return _camera
 
     @staticmethod
     @jaxtyped
+    @add_tracing_name
     def create_buffers(
         width: int,
         height: int,
         batch: Optional[int] = None,
         colour_default: Colour = jnp.array((1., 1., 1.), dtype=jnp.single),
         zbuffer_default: Num[Array, ""] = jnp.array(1, dtype=jnp.single),
     ) -> Buffers:
@@ -176,32 +179,40 @@
             targets=(canvas, ),
         )
 
         return buffers
 
     @classmethod
     @jaxtyped
-    @partial(jax.jit, static_argnames=("cls", ), donate_argnums=(4, ))
+    @partial(
+        jax.jit,
+        static_argnames=("cls", "loop_unroll"),
+        donate_argnums=(4, ),
+        inline=True,
+    )
+    @add_tracing_name
     def render(
         cls,
         model: MergedModel,
         light: LightParameters,
         camera: Camera,
         buffers: Buffers,
         shadow_param: Optional[ShadowParameters] = None,
+        loop_unroll: int = 1,
     ) -> Buffers:
         """Render the scene with the given camera.
 
         Parameters:
           - model: merged model of all the objects to render.
           - light: the light to render the scene with.
           - camera: the camera to render the scene with.
           - buffers: the buffers to render the scene with.
           - shadow_param: the shadow parameters to render the scene with. Keep
             it None to disable shadows.
+          - loop_unroll: passed directly to `render`. See `pipeline:render`.
 
         Returns: Buffers, with zbuffer and (coloured image, ).
         """
         # flatten so each vertex has its own "extra"
         position = model.verts[model.faces.reshape((-1, ))]
         normal = model.norms[model.faces_norm.reshape((-1, ))]
         uv = model.uvs[model.faces_uv.reshape((-1, ))]
@@ -245,14 +256,15 @@
             # no shadows
             buffers = render(
                 camera=camera,
                 shader=PhongReflectionTextureShader,
                 buffers=buffers,
                 face_indices=face_indices,
                 extra=extra,
+                loop_unroll=loop_unroll,
             )
             assert isinstance(buffers, Buffers), f"{buffers}"
 
             return buffers
         else:
             # with shadows
             assert isinstance(shadow_param,
@@ -268,14 +280,15 @@
                 faces=model.faces,
                 light_direction=light.direction,
                 viewport_matrix=camera.viewport,
                 centre=shadow_param.centre,
                 up=shadow_param.up,
                 strength=shadow_param.strength,
                 offset=shadow_param.offset,
+                loop_unroll=loop_unroll,
             )
             assert isinstance(shadow, Shadow), f"{shadow}"
 
             _extra = PhongReflectionShadowTextureExtraInput(
                 **extra._asdict(),
                 shadow=shadow,
                 camera=camera,
@@ -284,45 +297,55 @@
             # second pass: actual rendering
             buffers = render(
                 camera=camera,
                 shader=PhongReflectionShadowTextureShader,
                 buffers=buffers,
                 face_indices=face_indices,
                 extra=_extra,
+                loop_unroll=loop_unroll,
             )
             assert isinstance(buffers, Buffers), f"{buffers}"
 
             return buffers
 
     @classmethod
     @jaxtyped
+    @partial(
+        jax.jit,
+        static_argnames=("cls", "width", "height", "loop_unroll"),
+        inline=True,
+    )
+    @add_tracing_name
     def get_camera_image(
         cls,
         objects: Sequence[ModelObject],
         light: LightParameters,
         camera: Union[Camera, CameraParameters],
         width: int,
         height: int,
         colour_default: Colour = jnp.array((1., 1., 1.), dtype=jnp.single),
         zbuffer_default: Num[Array, ""] = jnp.array(1, dtype=jnp.single),
         shadow_param: Optional[ShadowParameters] = None,
+        loop_unroll: int = 1,
     ) -> Canvas:
         """Render the scene with the given camera.
 
         The dtype of `colour_default` and `zbuffer_default` will be used as the
         dtype of canvas and zbuffer.
 
         Parameters:
           - objects: the objects to render.
           - light: the light to render the scene with.
           - camera: the camera to render the scene with.
           - width, height: the size of the image to render.
           - colour_default: default colours to fill the image with.
           - zbuffer_default: default zbuffer values to fill with.
           - shadow_param: the shadow parameters to render the scene with. Keep
+            it None to disable shadows.
+          - loop_unroll: passed directly to `render`. See `pipeline:render`.
 
         Returns: Buffers, with zbuffer and (coloured image, ).
         """
         _camera: Camera
         if isinstance(camera, CameraParameters):
             _camera = cls.create_camera_from_parameters(camera)
         else:
@@ -359,11 +382,12 @@
         canvas: Canvas
         _, (canvas, ) = cls.render(
             model=model,
             light=light,
             camera=_camera,
             buffers=buffers,
             shadow_param=shadow_param,
+            loop_unroll=loop_unroll,
         )
         assert isinstance(canvas, Canvas), f"{canvas}"
 
         return canvas
```

### Comparing `jaxrenderer-0.2.1/renderer/scene.py` & `jaxrenderer-0.3.0/renderer/scene.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.1/renderer/shaders/README.md` & `jaxrenderer-0.3.0/renderer/shaders/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.1/renderer/shaders/depth.py` & `jaxrenderer-0.3.0/renderer/shaders/depth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from functools import partial
 from typing import NamedTuple
 
 import jax
 from jaxtyping import Array, Float, jaxtyped
 
+from .._meta_utils import add_tracing_name
 from ..shader import ID, PerVertex, Shader
 from ..geometry import Camera, to_homogeneous
 from ..types import Vec4f
 
 jax.config.update('jax_array', True)
 
 
@@ -29,15 +31,16 @@
 
 class DepthShader(Shader[DepthExtraInput, DepthExtraFragmentData,
                          DepthExtraMixerOutput]):
     """Depth Shading."""
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: DepthExtraInput,
     ) -> tuple[PerVertex, DepthExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
```

### Comparing `jaxrenderer-0.2.1/renderer/shaders/gouraud.py` & `jaxrenderer-0.3.0/renderer/shaders/gouraud.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, jaxtyped
 
+from .._meta_utils import add_tracing_name
 from ..shader import ID, PerFragment, PerVertex, Shader
 from ..geometry import Camera, normalise, to_homogeneous
 from ..types import Colour, LightSource, Vec2f, Vec3f, Vec4f
 
 jax.config.update('jax_array', True)
 
 
@@ -37,15 +39,16 @@
 
 class GouraudShader(Shader[GouraudExtraInput, GouraudExtraFragmentData,
                            GouraudExtraMixerOutput]):
     """Gouraud Shading with simple parallel lighting."""
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: GouraudExtraInput,
     ) -> tuple[PerVertex, GouraudExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
@@ -69,15 +72,16 @@
         return (
             PerVertex(gl_Position=gl_Position),
             GouraudExtraFragmentData(colour=colour),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
         gl_FrontFacing: Bool[Array, ""],
         gl_PointCoord: Vec2f,
         varying: GouraudExtraFragmentData,
         extra: GouraudExtraInput,
     ) -> tuple[PerFragment, GouraudExtraFragmentData]:
```

### Comparing `jaxrenderer-0.2.1/renderer/shaders/gouraud_texture.py` & `jaxrenderer-0.3.0/renderer/shaders/gouraud_texture.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, jaxtyped
 
+from .._meta_utils import add_tracing_name
 from ..geometry import Camera, normalise, to_homogeneous
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
 from ..types import Colour, LightSource, Texture, Vec2f, Vec3f, Vec4f
 
 jax.config.update('jax_array', True)
 
 
@@ -44,15 +46,16 @@
 class GouraudTextureShader(Shader[GouraudTextureExtraInput,
                                   GouraudTextureExtraFragmentData,
                                   GouraudTextureExtraMixerOutput]):
     """Gouraud Shading with simple parallel lighting and texture."""
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: GouraudTextureExtraInput,
     ) -> tuple[PerVertex, GouraudTextureExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
@@ -79,15 +82,16 @@
                 colour=light_colour,
                 uv=extra.uv[gl_VertexID],
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
         gl_FrontFacing: Bool[Array, ""],
         gl_PointCoord: Vec2f,
         varying: GouraudTextureExtraFragmentData,
         extra: GouraudTextureExtraInput,
     ) -> tuple[PerFragment, GouraudTextureExtraFragmentData]:
@@ -119,15 +123,16 @@
                 colour=texture_colour * light_colour,
                 uv=varying.uv,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: GouraudTextureExtraFragmentData,
     ) -> tuple[MixerOutput, GouraudTextureExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: GouraudTextureExtraFragmentData
```

### Comparing `jaxrenderer-0.2.1/renderer/shaders/phong.py` & `jaxrenderer-0.3.0/renderer/shaders/phong.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, jaxtyped
 
+from .._meta_utils import add_tracing_name
 from ..geometry import Camera, normalise, to_homogeneous
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
 from ..types import Colour, LightSource, Texture, Vec2f, Vec3f, Vec4f
 
 jax.config.update('jax_array', True)
 
 
@@ -51,15 +53,16 @@
 class PhongTextureShader(Shader[PhongTextureExtraInput,
                                 PhongTextureExtraFragmentData,
                                 PhongTextureExtraMixerOutput]):
     """Phong Shading with simple parallel lighting and texture."""
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: PhongTextureExtraInput,
     ) -> tuple[PerVertex, PhongTextureExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
@@ -82,15 +85,16 @@
                 normal=normal,
                 uv=extra.uv[gl_VertexID],
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
         gl_FrontFacing: Bool[Array, ""],
         gl_PointCoord: Vec2f,
         varying: PhongTextureExtraFragmentData,
         extra: PhongTextureExtraInput,
     ) -> tuple[PerFragment, PhongTextureExtraFragmentData]:
@@ -128,15 +132,16 @@
                 uv=varying.uv,
                 normal=varying.normal,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: PhongTextureExtraFragmentData,
     ) -> tuple[MixerOutput, PhongTextureExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: PhongTextureExtraFragmentData
```

### Comparing `jaxrenderer-0.2.1/renderer/shaders/phong_darboux.py` & `jaxrenderer-0.3.0/renderer/shaders/phong_darboux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import Partial
 from jaxtyping import Array, Bool, Float, Integer, jaxtyped
 
+from .._meta_utils import add_tracing_name
 from ..geometry import (Camera, Interpolation, interpolate, normalise,
                         to_cartesian, to_homogeneous)
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
 from ..types import (Colour, FaceIndices, LightSource, NormalMap, Texture,
                      Triangle, Vec2f, Vec2i, Vec3f, Vec4f)
 
 jax.config.update('jax_array', True)
@@ -75,15 +77,16 @@
                                        PhongTextureDarbouxExtraFragmentData,
                                        PhongTextureDarbouxExtraMixerOutput]):
     """Phong Shading with simple parallel lighting and texture, normals are
         represented in tangent space (Darboux frame)."""
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: PhongTextureDarbouxExtraInput,
     ) -> tuple[PerVertex, PhongTextureDarbouxExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
@@ -128,15 +131,16 @@
                 triangle=triangle_ndc,
                 triangle_uv=triangle_uv,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def interpolate(
         values: PhongTextureDarbouxExtraFragmentData,
         barycentric_screen: Vec3f,
         barycentric_clip: Vec3f,
     ) -> PhongTextureDarbouxExtraFragmentData:
         smooth_interpolation = Partial(
             interpolate,
@@ -163,15 +167,16 @@
         assert isinstance(varying.triangle, Triangle3f)
         assert isinstance(varying.triangle_uv, Triangle2f)
 
         return varying
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
         gl_FrontFacing: Bool[Array, ""],
         gl_PointCoord: Vec2f,
         varying: PhongTextureDarbouxExtraFragmentData,
         extra: PhongTextureDarbouxExtraInput,
     ) -> tuple[PerFragment, PhongTextureDarbouxExtraFragmentData]:
@@ -232,15 +237,16 @@
                 lambda: texture_colour * light_colour,
                 lambda: jnp.zeros(3),
             )),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: PhongTextureDarbouxExtraFragmentData,
     ) -> tuple[MixerOutput, PhongTextureDarbouxExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: PhongTextureDarbouxExtraFragmentData
```

### Comparing `jaxrenderer-0.2.1/renderer/shaders/phong_reflection.py` & `jaxrenderer-0.3.0/renderer/shaders/phong_reflection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, Integer, jaxtyped
 
+from .._meta_utils import add_tracing_name
 from ..geometry import Camera, normalise, to_homogeneous
 from ..model import MergedModel
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
 from ..types import (Colour, LightSource, SpecularMap, Texture, Vec2f, Vec2i,
                      Vec3f, Vec4f)
 
 jax.config.update('jax_array', True)
@@ -71,15 +73,16 @@
         Shader[PhongReflectionTextureExtraInput,
                PhongReflectionTextureExtraFragmentData,
                PhongReflectionTextureExtraMixerOutput]):
     """PhongReflection Shading with simple parallel lighting and texture."""
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: PhongReflectionTextureExtraInput,
     ) -> tuple[PerVertex, PhongReflectionTextureExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
@@ -104,15 +107,16 @@
                 uv=extra.uv[gl_VertexID],
                 texture_index=extra.texture_index[gl_VertexID],
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def interpolate(
         values: PhongReflectionTextureExtraFragmentData,
         barycentric_screen: Vec3f,
         barycentric_clip: Vec3f,
     ) -> PhongReflectionTextureExtraFragmentData:
         varying = Shader.interpolate(
             values=values,
@@ -123,15 +127,16 @@
         varying = varying._replace(texture_index=values.texture_index[0])
         assert isinstance(varying, PhongReflectionTextureExtraFragmentData)
 
         return varying
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
         gl_FrontFacing: Bool[Array, ""],
         gl_PointCoord: Vec2f,
         varying: PhongReflectionTextureExtraFragmentData,
         extra: PhongReflectionTextureExtraInput,
     ) -> tuple[PerFragment, PhongReflectionTextureExtraFragmentData]:
@@ -182,27 +187,24 @@
 
         return (
             PerFragment(
                 keeps=jnp.logical_and(built_in.keeps, gl_FrontFacing),
                 use_default_depth=built_in.use_default_depth,
             ),
             PhongReflectionTextureExtraFragmentData(
-                colour=lax.cond(
-                    (colour >= 0).all(),
-                    lambda: colour,
-                    lambda: jnp.zeros(3),
-                ),
+                colour=colour,
                 uv=varying.uv,
                 normal=varying.normal,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: PhongReflectionTextureExtraFragmentData,
     ) -> tuple[MixerOutput, PhongReflectionTextureExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: PhongReflectionTextureExtraFragmentData
```

### Comparing `jaxrenderer-0.2.1/renderer/shaders/phong_reflection_shadow.py` & `jaxrenderer-0.3.0/renderer/shaders/phong_reflection_shadow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from functools import partial
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, Integer, jaxtyped
 
+from .._meta_utils import add_tracing_name
 from ..geometry import Camera, normalise, normalise_homogeneous, to_homogeneous
 from ..model import MergedModel
 from ..shader import ID, MixerOutput, PerFragment, PerVertex, Shader
 from ..shadow import Shadow
 from ..types import (Colour, LightSource, SpecularMap, Texture, Vec2f, Vec2i,
                      Vec3f, Vec4f)
 
@@ -81,15 +83,16 @@
                PhongReflectionShadowTextureExtraMixerOutput]):
     """Phong Shading with simple parallel lighting, texture, Phong Reflection
         approximation and ShadowMap.
     """
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def vertex(
         gl_VertexID: ID,
         gl_InstanceID: ID,
         camera: Camera,
         extra: PhongReflectionShadowTextureExtraInput,
     ) -> tuple[PerVertex, PhongReflectionShadowTextureExtraFragmentData]:
         # Use gl_VertexID to index in `extra` buffer.
@@ -120,15 +123,16 @@
                 texture_index=extra.texture_index[gl_VertexID],
                 shadow_coord=shadow_coord,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def interpolate(
         values: PhongReflectionShadowTextureExtraFragmentData,
         barycentric_screen: Vec3f,
         barycentric_clip: Vec3f,
     ) -> PhongReflectionShadowTextureExtraFragmentData:
         varying = Shader.interpolate(
             values=values,
@@ -140,15 +144,16 @@
         assert isinstance(varying,
                           PhongReflectionShadowTextureExtraFragmentData)
 
         return varying
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def fragment(
         gl_FragCoord: Vec4f,
         gl_FrontFacing: Bool[Array, ""],
         gl_PointCoord: Vec2f,
         varying: PhongReflectionShadowTextureExtraFragmentData,
         extra: PhongReflectionShadowTextureExtraInput,
     ) -> tuple[PerFragment, PhongReflectionShadowTextureExtraFragmentData]:
@@ -216,27 +221,24 @@
 
         return (
             PerFragment(
                 keeps=jnp.logical_and(built_in.keeps, gl_FrontFacing),
                 use_default_depth=built_in.use_default_depth,
             ),
             PhongReflectionShadowTextureExtraFragmentData(
-                colour=lax.cond(
-                    (colour >= 0).all(),
-                    lambda: colour,
-                    lambda: jnp.zeros(3),
-                ),
+                colour=colour,
                 uv=varying.uv,
                 normal=varying.normal,
             ),
         )
 
     @staticmethod
     @jaxtyped
-    @jax.jit
+    @partial(jax.jit, inline=True)
+    @add_tracing_name
     def mix(
         gl_FragDepth: Float[Array, "primitives"],
         keeps: Bool[Array, "primitives"],
         extra: PhongReflectionShadowTextureExtraFragmentData,
     ) -> tuple[MixerOutput, PhongReflectionShadowTextureExtraMixerOutput]:
         mixer_output: MixerOutput
         extra_output: PhongReflectionShadowTextureExtraFragmentData
```

### Comparing `jaxrenderer-0.2.1/renderer/shadow.py` & `jaxrenderer-0.3.0/renderer/shadow.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import NamedTuple
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Float, jaxtyped
 
+from ._meta_utils import add_tracing_name
 from .geometry import Camera, View, Viewport
 from .pipeline import render
 from .shaders.depth import DepthExtraInput, DepthShader
 from .types import (Buffers, Colour, FaceIndices, Vec2f, Vec2i, Vec3f,
                     Vertices, ZBuffer)
 
 
@@ -23,26 +24,33 @@
     shadowed colour.
     """
     camera: Camera
     """Camera from world space to shadow map's screen space."""
 
     @staticmethod
     @jaxtyped
-    @partial(jax.jit, donate_argnums=(0, ))
+    @partial(
+        jax.jit,
+        static_argnames=("loop_unroll", ),
+        donate_argnums=(0, ),
+        inline=True,
+    )
+    @add_tracing_name
     def render_shadow_map(
         shadow_map: ZBuffer,
         verts: Vertices,
         faces: FaceIndices,
         light_direction: Vec3f,
         viewport_matrix: Viewport,
         centre: Vec3f,
         up: Vec3f,
         strength: Colour,
         offset: float = 0.001,
         distance: float = 10.,
+        loop_unroll: int = 1,
     ) -> "Shadow":
         """Render shadow map from light source's point of view.
 
         Parameters:
           - shadow_map: ZBuffer to store the depth map.
           - verts: vertices of the object.
           - faces: face indices of the object.
@@ -53,14 +61,15 @@
           - up: up direction of the scene, same as object's camera's up.
           - strength: strength of shadow. For details, see `Shadow.strength`.
           - offset: Offset to avoid self-shadowing / z-fighting. This will be
             added to the shadow map, making the shadows further away from
             the light.
           - distance: Distance from the light source to the centre of the
             scene. This is mainly to avoid objects being clipped.
+          - loop_unroll: passed directly to `render`. See `pipeline:render`.
 
         Returns: Updated `Shadow` object with shadow_map updated.
         """
 
         view: View = Camera.view_matrix(
             # keep "forward = -light_direction"
             eye=centre + light_direction * distance,
@@ -81,43 +90,51 @@
             ),
             viewport=viewport_matrix,
         )
         assert isinstance(_camera, Camera)
 
         buffers = Buffers(zbuffer=shadow_map, targets=tuple())
         extra = DepthExtraInput(position=verts)
-        shadow_map, _ = render(_camera, DepthShader, buffers, faces, extra)
+        shadow_map, _ = render(
+            _camera,
+            DepthShader,
+            buffers,
+            faces,
+            extra,
+            loop_unroll=loop_unroll,
+        )
         shadow_map = shadow_map + offset
         assert isinstance(shadow_map, ZBuffer)
 
         shadow: Shadow = Shadow(
             shadow_map=shadow_map,
             strength=strength,
             camera=_camera,
         )
 
         return shadow
 
     @jaxtyped
     @partial(jax.jit, inline=True)
+    @add_tracing_name
     def get(self, position: Vec2f) -> Float[Array, ""]:
         """Get shadow depth at `position`.
 
         Parameters:
           - position: position in shadow buffer's screen space.
         """
         assert isinstance(position, Vec2f), f"{position} is not a Vec3f."
 
         pos: Vec2i = lax.round(position[:2]).astype(int)
         assert isinstance(pos, Vec2i)
 
-        value: Float[Array, ""] = lax.cond(
-            jnp.logical_or(
-                pos < 0,
-                pos >= jnp.asarray(self.shadow_map.shape[:2]),
-            ).any(),
-            lambda: jnp.inf,  # outside shadow map, no shadow
-            lambda: self.shadow_map[pos[0], pos[1]],
+        value: Float[Array, ""]
+        value = self.shadow_map.at[pos[0], pos[1]].get(
+            mode="fill",
+            indices_are_sorted=True,
+            unique_indices=True,
+            # outside shadow map, no shadow
+            fill_value=jnp.inf,
         )
         assert isinstance(value, Float[Array, ""])
 
         return value
```

### Comparing `jaxrenderer-0.2.1/renderer/shapes/capsule.py` & `jaxrenderer-0.3.0/renderer/shapes/capsule.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.1/renderer/shapes/cube.py` & `jaxrenderer-0.3.0/renderer/shapes/cube.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.1/renderer/types.py` & `jaxrenderer-0.3.0/renderer/types.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.1/renderer/utils.py` & `jaxrenderer-0.3.0/renderer/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+from functools import partial
 from typing import Sequence, Union
 
 import jax
 import jax.numpy as jnp
 from jax import lax
 from jaxtyping import Array, Integer, Num, Shaped, jaxtyped
 
+from ._meta_utils import add_tracing_name
 from .types import Canvas, Texture, ZBuffer
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def get_value_from_index(
     matrix: Shaped[Array, "width height batch *valueDimensions"],
     index: Integer[Array, "width height"],
 ) -> Shaped[Array, "width height *valueDimensions"]:
     """Retrieve value along 3rd axis using index value from index matrix."""
     return jax.vmap(jax.vmap(lambda mt, ix: mt[ix]))(matrix, index)
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def merge_canvases(
     zbuffers: Num[Array, "batch width height"],
     canvases: Shaped[Array, "batch width height channel"],
 ) -> tuple[ZBuffer, Canvas]:
     """Merge canvases by selecting each pixel with max z value in zbuffer,
         then merge zbuffer as well.
     """
@@ -43,15 +47,16 @@
     )
     assert isinstance(canvas, Canvas)
 
     return zbuffer, canvas
 
 
 @jaxtyped
-@jax.jit
+@partial(jax.jit, inline=True)
+@add_tracing_name
 def transpose_for_display(
     matrix: Num[Array, "fst snd *channel"],
     flip_vertical: bool = True,
 ) -> Num[Array, "snd fst *channel"]:
     """Transpose matrix for display.
 
     When flip_vertical is disabled, the matrix's origin ([0, 0]) is assumed to
@@ -65,14 +70,15 @@
     if flip_vertical:
         mat = mat[::-1, ...]
 
     return mat
 
 
 @jaxtyped
+@add_tracing_name
 def build_texture_from_PyTinyrenderer(
     texture: Union[Num[Array, "length"], Sequence[float]],
     width: int,
     height: int,
 ) -> Texture:
     """Build a texture from PyTinyrenderer's format.
```

### Comparing `jaxrenderer-0.2.1/renderer/value_checker.py` & `jaxrenderer-0.3.0/renderer/value_checker.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.1/PKG-INFO` & `jaxrenderer-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: jaxrenderer
-Version: 0.2.1
+Version: 0.3.0
 Summary: Jax implementation of rasterizer renderer.
 Home-page: https://github.com/JoeyTeng/jaxrenderer
 License: Apache-2.0
 Author: Joey Teng
 Author-email: joey.teng.dev@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
-Requires-Dist: jax (>=0.4.4,<0.5.0)
-Requires-Dist: jaxlib (>=0.4.4,<0.5.0)
+Requires-Dist: jax (>=0.3.25,<5.0.0)
+Requires-Dist: jaxlib (>=0.3.25,<5.0.0)
 Requires-Dist: jaxtyping (>=0.2.19,<0.3.0)
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/JoeyTeng/jaxrenderer/issues
 Project-URL: Repository, https://github.com/JoeyTeng/jaxrenderer
 Description-Content-Type: text/markdown
 
 # JAX Renderer
```

