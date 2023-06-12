# Comparing `tmp/trajectory_manifold-0.0.1.tar.gz` & `tmp/trajectory_manifold-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajectory_manifold-0.0.1.tar", last modified: Thu May 18 21:05:11 2023, max compression
+gzip compressed data, was "trajectory_manifold-0.0.2.tar", last modified: Mon Jun 12 16:50:32 2023, max compression
```

## Comparing `trajectory_manifold-0.0.1.tar` & `trajectory_manifold-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 helmuth   (1000) helmuth   (1000)        0 2023-05-18 21:05:11.081837 trajectory_manifold-0.0.1/
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     1071 2023-05-18 18:49:20.000000 trajectory_manifold-0.0.1/LICENSE
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     1158 2023-05-18 21:05:11.078504 trajectory_manifold-0.0.1/PKG-INFO
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)      303 2023-05-18 21:03:47.000000 trajectory_manifold-0.0.1/README.md
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     1043 2023-05-18 18:49:20.000000 trajectory_manifold-0.0.1/pyproject.toml
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)       38 2023-05-18 21:05:11.081837 trajectory_manifold-0.0.1/setup.cfg
-drwxr-xr-x   0 helmuth   (1000) helmuth   (1000)        0 2023-05-18 21:05:11.078504 trajectory_manifold-0.0.1/tests/
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     1895 2023-05-18 18:49:20.000000 trajectory_manifold-0.0.1/tests/test_helpers.py
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     1968 2023-05-18 18:49:20.000000 trajectory_manifold-0.0.1/tests/test_manifold.py
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)      936 2023-05-18 21:03:47.000000 trajectory_manifold-0.0.1/tests/test_optimize.py
-drwxr-xr-x   0 helmuth   (1000) helmuth   (1000)        0 2023-05-18 21:05:11.078504 trajectory_manifold-0.0.1/trajectory_manifold/
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)      190 2023-05-18 18:49:20.000000 trajectory_manifold-0.0.1/trajectory_manifold/__init__.py
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)    12450 2023-05-18 18:49:20.000000 trajectory_manifold-0.0.1/trajectory_manifold/estimation.py
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     3290 2023-05-18 18:49:20.000000 trajectory_manifold-0.0.1/trajectory_manifold/examples.py
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     8519 2023-05-18 18:49:20.000000 trajectory_manifold-0.0.1/trajectory_manifold/helpers.py
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     9727 2023-05-18 18:49:20.000000 trajectory_manifold-0.0.1/trajectory_manifold/manifold.py
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     4881 2023-05-18 21:03:47.000000 trajectory_manifold-0.0.1/trajectory_manifold/optimize.py
-drwxr-xr-x   0 helmuth   (1000) helmuth   (1000)        0 2023-05-18 21:05:11.078504 trajectory_manifold-0.0.1/trajectory_manifold.egg-info/
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)     1158 2023-05-18 21:05:11.000000 trajectory_manifold-0.0.1/trajectory_manifold.egg-info/PKG-INFO
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)      507 2023-05-18 21:05:11.000000 trajectory_manifold-0.0.1/trajectory_manifold.egg-info/SOURCES.txt
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)        1 2023-05-18 21:05:11.000000 trajectory_manifold-0.0.1/trajectory_manifold.egg-info/dependency_links.txt
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)       36 2023-05-18 21:05:11.000000 trajectory_manifold-0.0.1/trajectory_manifold.egg-info/requires.txt
--rw-r--r--   0 helmuth   (1000) helmuth   (1000)       20 2023-05-18 21:05:11.000000 trajectory_manifold-0.0.1/trajectory_manifold.egg-info/top_level.txt
+drwxrwxr-x   0 helmuth   (1002) helmuth   (1002)        0 2023-06-12 16:50:32.952789 trajectory_manifold-0.0.2/
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     1071 2023-06-01 20:29:49.000000 trajectory_manifold-0.0.2/LICENSE
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     1323 2023-06-12 16:50:32.952789 trajectory_manifold-0.0.2/PKG-INFO
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)      468 2023-06-01 20:29:49.000000 trajectory_manifold-0.0.2/README.md
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     1073 2023-06-09 20:08:07.000000 trajectory_manifold-0.0.2/pyproject.toml
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)       38 2023-06-12 16:50:32.952789 trajectory_manifold-0.0.2/setup.cfg
+drwxrwxr-x   0 helmuth   (1002) helmuth   (1002)        0 2023-06-12 16:50:32.952789 trajectory_manifold-0.0.2/tests/
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     9218 2023-06-12 16:03:52.000000 trajectory_manifold-0.0.2/tests/test_estimation.py
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     2568 2023-06-12 16:25:33.000000 trajectory_manifold-0.0.2/tests/test_helpers.py
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     3983 2023-06-09 16:43:42.000000 trajectory_manifold-0.0.2/tests/test_manifold.py
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     3250 2023-06-12 15:45:24.000000 trajectory_manifold-0.0.2/tests/test_optimize.py
+drwxrwxr-x   0 helmuth   (1002) helmuth   (1002)        0 2023-06-12 16:50:32.952789 trajectory_manifold-0.0.2/trajectory_manifold/
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)      190 2023-06-01 20:29:49.000000 trajectory_manifold-0.0.2/trajectory_manifold/__init__.py
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)    13594 2023-06-12 15:50:40.000000 trajectory_manifold-0.0.2/trajectory_manifold/estimation.py
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     3290 2023-06-01 20:29:49.000000 trajectory_manifold-0.0.2/trajectory_manifold/examples.py
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)    10202 2023-06-12 16:29:26.000000 trajectory_manifold-0.0.2/trajectory_manifold/helpers.py
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)    11521 2023-06-09 16:54:57.000000 trajectory_manifold-0.0.2/trajectory_manifold/manifold.py
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     5704 2023-06-09 19:38:08.000000 trajectory_manifold-0.0.2/trajectory_manifold/optimize.py
+drwxrwxr-x   0 helmuth   (1002) helmuth   (1002)        0 2023-06-12 16:50:32.952789 trajectory_manifold-0.0.2/trajectory_manifold.egg-info/
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)     1323 2023-06-12 16:50:32.000000 trajectory_manifold-0.0.2/trajectory_manifold.egg-info/PKG-INFO
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)      532 2023-06-12 16:50:32.000000 trajectory_manifold-0.0.2/trajectory_manifold.egg-info/SOURCES.txt
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)        1 2023-06-12 16:50:32.000000 trajectory_manifold-0.0.2/trajectory_manifold.egg-info/dependency_links.txt
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)       36 2023-06-12 16:50:32.000000 trajectory_manifold-0.0.2/trajectory_manifold.egg-info/requires.txt
+-rw-rw-r--   0 helmuth   (1002) helmuth   (1002)       20 2023-06-12 16:50:32.000000 trajectory_manifold-0.0.2/trajectory_manifold.egg-info/top_level.txt
```

### Comparing `trajectory_manifold-0.0.1/LICENSE` & `trajectory_manifold-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectory_manifold-0.0.1/PKG-INFO` & `trajectory_manifold-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajectory_manifold
-Version: 0.0.1
+Version: 0.0.2
 Summary: Statistically Rigorous ODE Forecasting
 Author-email: Helmuth Naumer <hnaumer2@illinois.edu>
 Project-URL: Homepage, https://github.com/helmuthn/trajectory_manifold
 Project-URL: Documentation, https://www.helmuthnaumer.com/trajectory_manifold/
 Project-URL: Bug Tracker, https://github.com/helmuthn/trajectory_manifold/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,7 +20,9 @@
 # Trajectory Manifold
 
 [![Documentation](https://img.shields.io/badge/Documentation-Main-darkgreen)](https://www.helmuthnaumer.com/trajectory_manifold/)
 
 This repository contains code around statistical estimation on the trajectory manifold.
 
 It is intended to accompany a paper currently under review.
+
+The directory `figures` contains code to reproduce the figures in the work, while the directory `examples` contains the quick start example from the documentation.
```

### Comparing `trajectory_manifold-0.0.1/pyproject.toml` & `trajectory_manifold-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["trajectory_manifold"]
 
 [project]
 name = "trajectory_manifold"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Helmuth Naumer", email="hnaumer2@illinois.edu" },
 ]
 description = "Statistically Rigorous ODE Forecasting"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -29,7 +29,10 @@
     "jaxtyping"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/helmuthn/trajectory_manifold"
 "Documentation" = "https://www.helmuthnaumer.com/trajectory_manifold/"
 "Bug Tracker" = "https://github.com/helmuthn/trajectory_manifold/issues"
+
+[tool.ruff]
+ignore = ["F722"]
```

### Comparing `trajectory_manifold-0.0.1/tests/test_helpers.py` & `trajectory_manifold-0.0.2/tests/test_helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from trajectory_manifold.helpers import trapezoidal_inner_product
 from trajectory_manifold.helpers import trapezoidal_correlation
 from trajectory_manifold.helpers import apply_kernel_vec
+from trajectory_manifold.helpers import trapezoidal_pytree_vector_product
 
 import jax.numpy as jnp
+from jax import jit
 
 class Test_trapezoidal_inner_product:
     def test_trapezoidal_norm(self):
         """Tests inner product of x**2 with itself"""
         x = jnp.asarray([(i/1000.0)**2 for i in range(1001)])
         x = jnp.expand_dims(x, 1)
         stepsize = 1/1000.0
@@ -47,8 +49,26 @@
         dimensions = 3
         x = jnp.ones((functions, time_steps, dimensions))
         kernel = jnp.ones((time_steps, dimensions, dimensions))
 
         out = apply_kernel_vec(x, kernel)
         truth = 3 * jnp.ones((functions, time_steps, dimensions))
         assert (out == truth).all()
-        
+        
+
+class Test_trapezoidal_pytree_vector_product:
+    def test_basic(self):
+        y = jnp.ones((5,2))
+        X = (jnp.ones((5,2)), jnp.zeros((5,2)))
+        step_size = 1
+        result = trapezoidal_pytree_vector_product(y, X, step_size)
+        assert result[0] == 8
+        assert result[1] == 0
+
+    def test_jit(self):
+        y = jnp.ones((5,2))
+        X = (jnp.ones((5,2)), jnp.zeros((5,2)))
+        step_size = 1
+        j_test = jit(trapezoidal_pytree_vector_product)
+        result = j_test(y, X, step_size)
+        assert result[0] == 8
+        assert result[1] == 0
```

### Comparing `trajectory_manifold-0.0.1/trajectory_manifold/estimation.py` & `trajectory_manifold-0.0.2/trajectory_manifold/estimation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,278 +1,304 @@
 """This module includes functions for statistical estimation"""
 
 from typing import Callable
-from jaxtyping import Float, Array
+from jaxtyping import Float, Array, PyTree
 import jax
 from .manifold import system_pushforward_weight, SolverParameters
-from diffrax import ODETerm, SaveAt, PIDController, diffeqsolve
+from diffrax import ODETerm, SaveAt, diffeqsolve
 import jax.numpy as jnp
 
 def trajectory_log_likelihood(
-    vector_field: Callable[[any, Float[Array, " dim"], any], Float[Array, " dim"]], 
+    vector_field: Callable[[any, Float[Array, " dim"], PyTree], Float[Array, " dim"]], 
     observations: Float[Array, " timesteps dim2"],
     observation_times: Float[Array, " timesteps"],
     observation_log_likelihood: Callable[[Float[Array, " dim2"], Float[Array, " dim"]], float],
     parameters: SolverParameters,
-) -> Callable[[Float[Array, " dim"]], float]:
+) -> Callable[[Float[Array, " dim"], PyTree], Float]:
     """Constructs a likelihood function for a set of observations of a system.
     
     Given a representation of a differential equation, a set of observation 
     times and an observation likelihood function dependent on the state, 
     construct a likelihood function jointly over all observations.
     
     Args:
         vector_field: Governing differential equation mapping the current state
           to the derivative.
         observations: An N by K dimensional array of observations.
         observation_times: An N dimensional array of observation times.
         observation_likelihood: A function mapping pairs of states and 
           observations to the likelihood.
+        parameters: Parameters for the ODE solver
 
     Returns:
-        A function mapping the state at the initial observation time to the 
-        likelihood of the observation.
+        A function mapping the state and parameters at the initial observation 
+        time to the log likelihood of the observation.
     """
 
-    def likelihood(state: Float[Array, " dim"]) -> float:
-        term = ODETerm(vector_field)
-        solver = parameters.solver
-        saveat = SaveAt(ts = observation_times)
-        stepsize_controller = PIDController(rtol = parameters.relative_tolerance,
-                                            atol = parameters.absolute_tolerance)
-        
+    term = ODETerm(vector_field)
+    solver = parameters.solver
+    saveat = SaveAt(ts = observation_times)
+    stepsize_controller = parameters.stepsize_controller
+    t0 = parameters.time_interval[0]
+    t1 = parameters.time_interval[1]
+    dt0 = parameters.step_size_internal
+    max_steps = parameters.max_steps
+
+    def likelihood(state: Float[Array, " dim"],
+                   system_parameters: Float[Array, " dim3"]
+        ) -> Float:
+
         states = diffeqsolve(term,
                              solver,
-                             t0 = parameters.time_interval[0],
-                             t1 = parameters.time_interval[1],
-                             dt0 = 0.1,
+                             args = system_parameters,
+                             t0 = t0,
+                             t1 = t1,
+                             dt0 = dt0,
                              saveat = saveat,
                              stepsize_controller = stepsize_controller,
                              y0 = state,
-                             max_steps=parameters.max_steps).ys
+                             max_steps=max_steps).ys
 
         likelihood_v = jax.vmap(observation_log_likelihood)
 
         return jnp.sum(likelihood_v(observations, states))
     
     return likelihood
 
 def trajectory_likelihood(
-    vector_field: Callable[[any, Float[Array, " dim"], any], Float[Array, " dim"]], 
+    vector_field: Callable[[any, Float[Array, " dim"], PyTree], Float[Array, " dim"]], 
     observations: Float[Array, " timesteps dim2"],
     observation_times: Float[Array, " timesteps"],
     observation_likelihood: Callable[[Float[Array, " dim2"], Float[Array, " dim"]], float],
     parameters: SolverParameters,
-) -> Callable[[Float[Array, " dim"]], float]:
+) -> Callable[[Float[Array, " dim"], PyTree], Float]:
     """Constructs a likelihood function for a set of observations of a system.
     
     Given a representation of a differential equation, a set of observation 
     times and an observation likelihood function dependent on the state, 
     construct a likelihood function jointly over all observations.
     
     Args:
         vector_field: Governing differential equation mapping the current state
           to the derivative.
         observations: An N by K dimensional array of observations.
         observation_times: An N dimensional array of observation times.
         observation_likelihood: A function mapping pairs of states and 
           observations to the likelihood.
+        parameters: Parameters for the ODE solver
 
     Returns:
-        A function mapping the state at the initial observation time to the 
-        likelihood of the observation.
+        A function mapping the state and parameters at the initial observation 
+        time to the likelihood of the observation.
     """
 
-    def likelihood(state: Float[Array, " dim"]) -> float:
+    def likelihood(state: Float[Array, " dim"],
+                   system_parameters: Float[Array, " dim3"]
+        ) -> Float:
         term = ODETerm(vector_field)
         solver = parameters.solver
         saveat = SaveAt(ts = observation_times)
-        stepsize_controller = PIDController(rtol = parameters.relative_tolerance,
-                                            atol = parameters.absolute_tolerance)
+        stepsize_controller = parameters.stepsize_controller
         
         states = diffeqsolve(term,
                              solver,
+                             args = system_parameters,
                              t0 = parameters.time_interval[0],
                              t1 = parameters.time_interval[1],
-                             dt0 = 0.1,
+                             dt0 = parameters.step_size_internal,
                              saveat = saveat,
                              stepsize_controller = stepsize_controller,
                              y0 = state,
                              max_steps=parameters.max_steps).ys
 
         likelihood_v = jax.vmap(observation_likelihood)
 
         return jnp.prod(likelihood_v(observations, states))
     
     return likelihood
 
 
 def state_log_posterior(
-    vector_field: Callable[[any, Float[Array, " dim"], any], Float[Array, " dim"]], 
+    vector_field: Callable[[any, Float[Array, " dim"], PyTree], Float[Array, " dim"]], 
     observations: Float[Array, " timesteps dim2"],
     observation_times: Float[Array, " timesteps"],
     observation_likelihood: Callable[[Float[Array, " dim2"], Float[Array, " dim"]], float],
-    state_log_prior: Callable[[Float[Array, " dim"]], float],
+    log_prior: Callable[[Float[Array, " dim"], PyTree], float],
     parameters: SolverParameters,
-) -> Callable[[Float[Array, " dim"]], float]:
+) -> Callable[[Float[Array, " dim"], PyTree], float]:
     """Constructs a posterior distribution for the initial state of the system.
     
     Given a representation of a differential equation, a set of observation 
     times and an observation likelihood function dependent on the state, 
     construct a posterior distribution jointly over all observations.
     
     Args:
         vector_field: Governing differential equation mapping the current state
           to the derivative.
         observations: An N by K dimensional array of observations.
         observation_times: An N dimensional array of observation times.
         observation_likelihood: A function mapping pairs of states and 
           observations to the likelihood.
-        state_prior: A function representing the prior distribution of the
-          state of the system at the initial observation time.
+        log_prior: A function representing the prior distribution of the
+          initial state and parameters of the system.
+        parameters: Parameters for the ODE solver
 
     Returns:
-        A function mapping the state at the initial observation time to the 
-        likelihood of the observation.
+        A function mapping the state and parameters at the initial observation 
+        time to the log posterior of the trajectory.
     """
     log_likelihood = trajectory_log_likelihood(vector_field, 
                                        observations,
                                        observation_times, 
                                        observation_likelihood,
                                        parameters)
 
     def log_posterior(
-        state: Float[Array, " dim"]
-    ) -> float:
-        return log_likelihood(state) + state_log_prior(state)
+        state: Float[Array, " dim"],
+        system_parameters: Float[Array, " dim3"]
+    ) -> Float:
+        return log_likelihood(state, system_parameters) \
+               + log_prior(state, parameters)
       
     return log_posterior
 
 def state_posterior(
-    vector_field: Callable[[any, Float[Array, " dim"], any], Float[Array, " dim"]], 
+    vector_field: Callable[[any, Float[Array, " dim"], PyTree], Float[Array, " dim"]], 
     observations: Float[Array, " timesteps dim2"],
     observation_times: Float[Array, " timesteps"],
     observation_likelihood: Callable[[Float[Array, " dim2"], Float[Array, " dim"]], float],
-    state_prior: Callable[[Float[Array, " dim"]], float],
-) -> Callable[[Float[Array, " dim"]], float]:
+    prior: Callable[[Float[Array, " dim"], PyTree], float],
+    parameters: SolverParameters
+) -> Callable[[Float[Array, " dim"], PyTree], Float]:
     """Constructs a posterior distribution for the initial state of the system.
     
     Given a representation of a differential equation, a set of observation 
     times and an observation likelihood function dependent on the state, 
     construct a posterior distribution jointly over all observations.
     
     Args:
         vector_field: Governing differential equation mapping the current state
           to the derivative.
         observations: An N by K dimensional array of observations.
         observation_times: An N dimensional array of observation times.
         observation_likelihood: A function mapping pairs of states and 
           observations to the likelihood.
-        state_prior: A function representing the prior distribution of the
-          state of the system at the initial observation time.
+        prior: A function representing the prior distribution of the
+          initial state and parameters of the system.
+        parameters: Parameters for the ODE solver
 
     Returns:
-        A function mapping the state at the initial observation time to the 
-        likelihood of the observation.
+        A function mapping the state and initial condition at the initial 
+        observation time to the posterior of the initial condition and parameters.
     """
     likelihood = trajectory_likelihood(vector_field, 
                                        observations,
                                        observation_times, 
-                                       observation_likelihood)
+                                       observation_likelihood,
+                                       parameters)
 
     def posterior(
-        state: Float[Array, " dim"]
-    ) -> float:
-        return likelihood(state) * state_prior(state)
+        state: Float[Array, " dim"],
+        system_parameters: Float[Array, " dim3"]
+    ) -> Float:
+        return likelihood(state, system_parameters) \
+                * prior(state, system_parameters)
       
     return posterior
 
 
 def trajectory_log_posterior(
-    vector_field: Callable[[any, Float[Array, " dim"], any], Float[Array, " dim"]], 
+    vector_field: Callable[[any, Float[Array, " dim"], PyTree], Float[Array, " dim"]], 
     observations: Float[Array, " timesteps dim2"],
     observation_times: Float[Array, " timesteps"],
     observation_likelihood: Callable[[Float[Array, " dim2"], Float[Array, " dim"]], float],
-    state_log_prior: Callable[[Float[Array, " dim"]], float],
+    log_prior: Callable[[Float[Array, " dim"], PyTree], float],
     time_interval: tuple[float, float],
     parameters: SolverParameters,
-) -> Callable[[Float[Array, " dim"]], float]:
+) -> Callable[[Float[Array, " dim"], PyTree], Float]:
     """Constructs a posterior distribution for system trajectories.
     
     Given a representation of a differential equation, a set of observation 
     times and an observation likelihood function dependent on the state, 
     construct a posterior distribution jointly over all observations.
     
     Args:
         vector_field: Governing differential equation mapping the current state
           to the derivative.
         observations: An N by K dimensional array of observations.
         observation_times: An N dimensional array of observation times.
         observation_likelihood: A function mapping pairs of states and 
           observations to the likelihood.
-        state_prior: A function representing the prior distribution of the
-          state of the system at the initial observation time.
+        prior: A function representing the prior distribution of the
+          initial state and parameters of the system.
         time_interval: Time interval for the trajectory manifold in the form
           (initial time, final time).
+        parameters: Parameters for the ODE solver
 
     Returns:
-        A function mapping the state at the initial observation time to the 
-        posterior distribution of the observation.
+        A function mapping the state and system parameters at the initial 
+        observation time to the posterior distribution of the trajectory.
     """
     log_posterior = state_log_posterior(vector_field,
                                 observations,
                                 observation_times,
                                 observation_likelihood,
-                                state_log_prior,
+                                log_prior,
                                 parameters)
     
-    def weight(initial_condition):
+    def weight(initial_condition, system_parameters):
         return system_pushforward_weight(vector_field,
                                          time_interval,
-                                         initial_condition)
+                                         initial_condition,
+                                         system_parameters)
     
       
-    return lambda state: log_posterior(state) - jnp.log(weight(state))
+    return lambda state, params: log_posterior(state, params) \
+                                - jnp.log(weight(state, params))
 
 def trajectory_posterior(
-    vector_field: Callable[[any, Float[Array, " dim"], any], Float[Array, " dim"]], 
+    vector_field: Callable[[any, Float[Array, " dim"], PyTree], Float[Array, " dim"]], 
     observations: Float[Array, " timesteps dim2"],
     observation_times: Float[Array, " timesteps"],
     observation_likelihood: Callable[[Float[Array, " dim2"], Float[Array, " dim"]], float],
-    state_prior: Callable[[Float[Array, " dim"]], float],
+    prior: Callable[[Float[Array, " dim"], PyTree], float],
     time_interval: tuple[float, float],
-) -> Callable[[Float[Array, " dim"]], float]:
+    parameters: SolverParameters,
+) -> Callable[[Float[Array, " dim"], PyTree], Float]:
     """Constructs a posterior distribution for system trajectories.
     
     Given a representation of a differential equation, a set of observation 
     times and an observation likelihood function dependent on the state, 
     construct a posterior distribution jointly over all observations.
     
     Args:
         vector_field: Governing differential equation mapping the current state
           to the derivative.
         observations: An N by K dimensional array of observations.
         observation_times: An N dimensional array of observation times.
         observation_likelihood: A function mapping pairs of states and 
           observations to the likelihood.
-        state_prior: A function representing the prior distribution of the
-          state of the system at the initial observation time.
+        prior: A function representing the prior distribution of the
+          initial state and parameters of the system.
         time_interval: Time interval for the trajectory manifold in the form
           (initial time, final time).
+        parameters: Parameters for the ODE solver
 
     Returns:
         A function mapping the state at the initial observation time to the 
         posterior distribution of the observation.
     """
     posterior = state_posterior(vector_field,
                                 observations,
                                 observation_times,
                                 observation_likelihood,
-                                state_prior)
+                                prior,
+                                parameters)
     
-    def weight(initial_condition):
+    def weight(initial_condition, system_parameters):
         return system_pushforward_weight(vector_field,
                                          time_interval,
-                                         initial_condition)
+                                         initial_condition,
+                                         system_parameters)
     
       
-    return lambda state: posterior(state) * weight(state)
+    return lambda state, params: posterior(state, params) / weight(state, params)
```

### Comparing `trajectory_manifold-0.0.1/trajectory_manifold/examples.py` & `trajectory_manifold-0.0.2/trajectory_manifold/examples.py`

 * *Files identical despite different names*

### Comparing `trajectory_manifold-0.0.1/trajectory_manifold/helpers.py` & `trajectory_manifold-0.0.2/trajectory_manifold/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """This module contains linear algebra helper functions.
 
 The purpose of this module is to adapt standard linear algebra
 fuctions to the needs of this project. These include items such
 as computation of an inner product through the trapezoidal rule.
 """
 
-from jax import jit, vmap
-from jax.lax import fori_loop
+from jax import jit, vmap, tree_map
+from jax.lax import fori_loop, cond
 import jax.numpy as jnp
 
-from jaxtyping import Float, Array
+
+from jaxtyping import Float, Array, PyTree
 
 @jit
 def frobenius_inner_product(
     x: Float[Array, " *dim"], 
     y: Float[Array, " *dim"], 
 ) -> Float:
     """Computes the Frobenius inner product of two matrices.
@@ -55,14 +56,48 @@
     """
 
     out = (jnp.dot(x[0, :],  y[0, :]) + jnp.dot(x[-1, :], y[-1, :])) / 2
     out += frobenius_inner_product(x[1:-1, :], y[1:-1, :])
     return out * step_size
     
 
+def trapezoidal_pytree_vector_product(
+        y: Float[Array, " timesteps dim"],
+        X: PyTree,
+        step_size: Float,
+    ) -> PyTree:
+    """Computes the pytree-vector product where leaves are sampled functions.
+    
+    Given a PyTree where leaves are 2-dimensional arrays representing
+    sampled function and another 2-dimensional array reepresenting
+    a single multivariate function, returns a PyTree of the same shape
+    as the original input with leaves resulting from the L2 inner
+    products with the function.
+    
+    Args:
+        y: A 2D array with indices (timestep, dim)
+        X: A PyTree where leaves are 2D arrays with indices (timestep, dim)
+        step_size: Step size required for numerical integration scaling
+    
+    Returns:
+        A PyTree of the same shape a `X`, but with results of inner products
+        as leaves.
+    """
+
+    def is_leaf(x):
+        return isinstance(x, jnp.ndarray) \
+           and len(x.shape) == 2 \
+           and jnp.issubdtype(x.dtype, jnp.number)
+
+    @jit
+    def apply_vector(x):
+        return trapezoidal_inner_product(x, y, step_size)
+
+    return tree_map(apply_vector, X, is_leaf=is_leaf)
+
 @jit
 def trapezoidal_matrix_product(
     X: Float[Array, " functions1 timesteps dim"],
     Y: Float[Array, " functions2 timesteps dim"],
     step_size: Float,
 ) -> Float[Array, " functions1 functions2"]:
     """Computes the product of two matrices where rows represent functions.
@@ -77,14 +112,15 @@
         Y: An M by N by K array of N samples of each of M functions
           taking values in a K-dimensional space. 
         step_size: Spacing between sample points in the functions.
 
     Returns:
         The result of the generalized matrix-matrix product.
     """
+
     vv = lambda x, y: trapezoidal_inner_product(x, y, step_size)
     mv = vmap(vv, (0, None), 0)
     mm = vmap(mv, (None, 0), 1)
     return mm(X, Y)
     
 
 @jit
@@ -182,14 +218,16 @@
     Returns:
         An M by M matrix where the (i,j)'th element is the approximate
         inner product between rows i and j of the input matrix. 
     """
 
     M = U.shape[0]
     out = jnp.zeros((M, M))
+    if M == 0:
+        return out
 
     def inner(i, val):
         out, U, step_size = val
 
         def inner2(j, val):
             out, U, step_size, i = val
             value = trapezoidal_inner_product(U[i,...], U[j,...], step_size)
@@ -251,8 +289,23 @@
 
         out, U, step_size, i = fori_loop(i, M, inner2, (out, U, step_size, i))
 
         return out, U, step_size
 
     out, U, step_size = fori_loop(0, M, inner, (out, U, step_size))
 
-    return out
+    return out
+
+@jit
+def safe_det(A: Float[Array, " dim dim"]):
+    """Return the determinant with an empty matrix set to 1
+    
+    Used for computing the determinants of block diagonal matrices
+    in the case where a block size may be zero
+    
+    Args:
+        A: A matrix to compute the determinant
+        
+    Returns:
+        The determinant of the matrix, or 1 if the matrix is empty
+    """
+    return cond(A.shape[0] == 0, lambda x: 1.0, jnp.linalg.det, A)
```

### Comparing `trajectory_manifold-0.0.1/trajectory_manifold/manifold.py` & `trajectory_manifold-0.0.2/trajectory_manifold/manifold.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,53 +7,57 @@
 
 from jax import jit, jacrev
 import jax.numpy as jnp
 
 from jaxtyping import Float, Array, PyTree
 from typing import Callable
 
-from diffrax import AbstractSolver, Tsit5, Heun
+from diffrax import AbstractSolver, Heun
 from diffrax import ODETerm, SaveAt, PIDController, diffeqsolve
+from diffrax import AbstractStepSizeController
 
 from functools import partial
 from typing import NamedTuple
 
 from .helpers import trapezoidal_correlation, trapezoidal_correlation_weighted
+from .helpers import safe_det
 
 
 class SolverParameters(NamedTuple):
     """Stores Information for ODE Solvers.
     
     Records the parameters for solving an ODE using Diffrax,
     including the solver, tolerances, output grid size, and time horizon.
     
     Attributes:
-        relative_tolerance: Relative tolerance for the ODE solution.
-        absolute_tolerance: Absolute tolerance for the ODE solution.
-        step_size: Output mesh size. Note: Does not impact internal computations.
+        stepsize_controller: Absolute tolerance for the ODE solution.
+        step_size_internal: Internal mesh size for constant step size controller.
+        step_size_output: Output mesh size. Note: Does not impact internal computations.
         time_interval: Tuple of (initial time, final time). The interval is 
           inclusive of the initial time, but exclusive of the final time.
         solver: The particular ODE solver to use.
         max_steps: Max steps for the solver.
     """
 
-    relative_tolerance: float
-    absolute_tolerance: float
-    step_size: float
-    time_interval: tuple[float, float]
+    stepsize_controller: AbstractStepSizeController
+    step_size_internal: Float
+    step_size_output: Float
+    time_interval: tuple[Float, Float]
     solver: AbstractSolver
     max_steps: int
 
 
-@partial(jit, static_argnames=['vector_field', 'parameters'])
+@partial(jit, static_argnames=['vector_field', 'solver_parameters'])
 def system_sensitivity_and_solution(
     vector_field: Callable[[Float, Float[Array, " dim"], PyTree], Float[Array, " dim"]], 
     initial_condition: Float[Array, " dim"],
-    parameters: SolverParameters,
-) -> Float[Array, " dim timesteps dim"]:
+    system_parameters: PyTree,
+    solver_parameters: SolverParameters,
+) -> tuple[tuple[Float[Array, " dim timesteps dim"], PyTree],
+           Float[Array, " timesteps dim"]]:
     """Computes the differential equation sensitivity to the initial conditions.
     
     Given a differential equation, initial condition, and desired time horizon,
     computes the Jacobian of the transformation from the initial condition
     to the Riemannian manifold of valid trajectories. The Jacobian is expressed
     in the ambient space of square integrable functions.
     
@@ -70,177 +74,202 @@
         sensitivity: A matrix where each row represents the sensitivity of the 
           system solution to a perturbation along some element of an orthonormal 
           basis of the state space.
         solution: A matrix representing the corresponding solution of the ODE
     """
 
     term = ODETerm(vector_field)
-    solver = parameters.solver
-    timesteps = jnp.arange(parameters.time_interval[0], 
-                           parameters.time_interval[1], 
-                           step=parameters.step_size)
+    solver = solver_parameters.solver
+    timesteps = jnp.arange(solver_parameters.time_interval[0], 
+                           solver_parameters.time_interval[1], 
+                           step=solver_parameters.step_size_output)
 
     saveat = SaveAt(ts = timesteps)
-    stepsize_controller = PIDController(rtol = parameters.relative_tolerance,
-                                        atol = parameters.absolute_tolerance)
+    stepsize_controller = solver_parameters.stepsize_controller
 
     @jit
     def diffeq_solution(
         x0: Float[Array, " dim"],
+        p: PyTree
     ) -> Float[Array, " timesteps dim"]:
         """Returns the solution to the differential equation."""
         return diffeqsolve(term,
                            solver,
-                           t0 = parameters.time_interval[0],
-                           t1 = parameters.time_interval[1],
-                           dt0 = 0.1,
+                           t0  = solver_parameters.time_interval[0],
+                           t1  = solver_parameters.time_interval[1],
+                           dt0 = solver_parameters.step_size_internal,
                            saveat = saveat,
                            stepsize_controller = stepsize_controller,
                            y0 = x0,
-                           max_steps=parameters.max_steps).ys
+                           args = p,
+                           max_steps = solver_parameters.max_steps).ys
+
+    solution = diffeq_solution(initial_condition, system_parameters)
+    sensitivity = jacrev(diffeq_solution, argnums=[0,1])(initial_condition, 
+                                                         system_parameters)
 
-    solution = diffeq_solution(initial_condition)
-    sensitivity = jacrev(diffeq_solution)(initial_condition)
+    if isinstance(system_parameters, jnp.ndarray):
+      sensitivity = (jnp.moveaxis(sensitivity[0], 2, 0), 
+                     jnp.moveaxis(sensitivity[1], 2, 0))
+    else:
+      sensitivity = (jnp.moveaxis(sensitivity[0], 2, 0), 
+                     sensitivity[1])
 
-    return jnp.moveaxis(sensitivity, 2, 0), solution
+    return (sensitivity, solution)
 
 
-@partial(jit, static_argnames=['vector_field', 'parameters'])
+@partial(jit, static_argnames=['vector_field', 'solver_parameters'])
 def system_sensitivity(
     vector_field: Callable[[Float, Float[Array, " dim"], PyTree], Float[Array, " dim"]], 
     initial_condition: Float[Array, " dim"],
-    parameters: SolverParameters,
+    system_parameters: PyTree,
+    solver_parameters: SolverParameters,
 ) -> Float[Array, " dim timesteps dim"]:
     """Computes the differential equation sensitivity to the initial conditions.
     
     Given a differential equation, initial condition, and desired time horizon,
     computes the Jacobian of the transformation from the initial condition
     to the Riemannian manifold of valid trajectories. The Jacobian is expressed
     in the ambient space of square integrable functions.
     
     Args:
         vector_field: Governing differential equation mapping the current state
           to the derivative.
         initial_condition: The position in the statespace to be pushed onto 
           the manifold.
-        parameters: The set of parameters for the ODE solver.
+        system_parameters: The parameters for the vector field.
+        solver_parameters: The set of parameters for the ODE solver.
     
     Returns:
         A matrix where each row represents the sensitivity of the system solution
         to a perturbation along some element of an orthonormal basis of the
         state space.
     """
 
     term = ODETerm(vector_field)
-    solver = parameters.solver
-    timesteps = jnp.arange(parameters.time_interval[0], 
-                           parameters.time_interval[1], 
-                           step=parameters.step_size)
+    solver = solver_parameters.solver
+    timesteps = jnp.arange(solver_parameters.time_interval[0], 
+                           solver_parameters.time_interval[1], 
+                           step=solver_parameters.step_size_output)
 
     saveat = SaveAt(ts = timesteps)
-    stepsize_controller = PIDController(rtol = parameters.relative_tolerance,
-                                        atol = parameters.absolute_tolerance)
+    stepsize_controller = solver_parameters.stepsize_controller
 
     @jit
     def diffeq_solution(
         x0: Float[Array, " dim"],
+        p: PyTree
     ) -> Float[Array, " timesteps dim"]:
         """Returns the solution to the differential equation."""
         return diffeqsolve(term,
                            solver,
-                           t0 = parameters.time_interval[0],
-                           t1 = parameters.time_interval[1],
-                           dt0 = 0.1,
+                           t0  = solver_parameters.time_interval[0],
+                           t1  = solver_parameters.time_interval[1],
+                           dt0 = solver_parameters.step_size_internal,
                            saveat = saveat,
                            stepsize_controller = stepsize_controller,
                            y0 = x0,
-                           max_steps=parameters.max_steps).ys
+                           args = p,
+                           max_steps=solver_parameters.max_steps).ys
 
-    sensitivity = jacrev(diffeq_solution)(initial_condition)
+    sensitivity = jacrev(diffeq_solution, argnums=[0,1])(initial_condition, 
+                                                         system_parameters)
+
+    if isinstance(system_parameters, jnp.ndarray):
+      return (jnp.moveaxis(sensitivity[0], 2, 0), jnp.moveaxis(sensitivity[1], 2, 0))
+    else:
+      return (jnp.moveaxis(sensitivity[0], 2, 0), sensitivity[1])
 
-    return jnp.moveaxis(sensitivity, 2, 0)
 
 @partial(jit, static_argnames=['vector_field', 'time_interval'])
 def system_pushforward_weight(
     vector_field: Callable[[Float, Float[Array, " dim"], PyTree], Float[Array, " dim"]], 
     time_interval: tuple[float, float], 
     initial_condition: Float[Array, " dim"],
+    system_parameters: Float[Array, " dim2"],
 ) -> Float:
     """Computes the pushforward weight for a given initial condition.
     
     Given a differential equation, initial condition, and desired time horizon,
     computes the weight required to push densities onto the Riemannian manifold
     of valid trajectories of the system.
     
     Args:
         vector_field: Governing differential equation mapping the current state
           to the derivative.
         time_interval: Time interval for the trajectory manifold in the form
           (initial time, final time).
-        initial_conditon: The position in the statespace to be pushed onto 
+        initial_condition: The position in the statespace to be pushed onto 
           the manifold.
+        system_parameters: The parameters for the vector field.
         
     Returns:
         The weight required to push a density onto the trajectory manifold.
     """
 
     absolute_tolerance = 1e-2
     relative_tolerance = 1e-2
     max_steps = 16**4
     step_size = 0.01
     solver = Heun()
-    parameters = SolverParameters(relative_tolerance, 
-                                  absolute_tolerance, 
-                                  step_size, 
-                                  time_interval, 
-                                  solver,
-                                  max_steps)
+    parameters = SolverParameters(stepsize_controller=PIDController(rtol=relative_tolerance,
+                                                                    atol=absolute_tolerance),
+                                  step_size_internal=0.1,
+                                  step_size_output=step_size,
+                                  time_interval = time_interval,
+                                  solver=solver,
+                                  max_steps = max_steps)
+
+    U = system_sensitivity(vector_field, initial_condition, system_parameters, parameters)
+    A = trapezoidal_correlation(U[0], step_size)
+    B = trapezoidal_correlation(U[1], step_size)
 
-    U = system_sensitivity(vector_field, initial_condition, parameters)
-    A = trapezoidal_correlation(U, step_size)
-
-    return jnp.sqrt(abs(jnp.linalg.det(A)))
+    return jnp.sqrt(abs(safe_det(A) * safe_det(B)))
 
 
 @partial(jit, static_argnames=['vector_field', 'time_interval'])
 def system_pushforward_weight_reweighted(
     vector_field: Callable[[any, Float[Array, " dim"], any], Float[Array, " dim"]], 
     time_interval: Float, 
     initial_condition: Float[Array, " dim"],
+    system_parameters: Float[Array, " dim2"],
     step_size: Float,
     kernel: Float[Array, " timesteps dim dim"]
 ) -> Float:
     """Computes the pushforward weight for a given initial condition.
     
     Given a differential equation, initial condition, and desired time horizon,
     computes the weight required to push densities onto the Riemannian manifold
     of valid trajectories of the system.
     
     Args:
         vector_field: Governing differential equation mapping the current state
           to the derivative.
         time_interval: Time interval for the trajectory manifold.
-        initial_conditon: The position in the statespace to be pushed onto 
+        initial_condition: The position in the statespace to be pushed onto 
           the manifold.
+        system_parameters: The parameters for the vector field.
         step_size: The step size for the numerical solution of the ODE.
         kernel: An N by K by K array of N timesteps of an integral kernel to
           apply to a K dimensional space.
         
     Returns:
         The weight required to push a density onto the trajectory manifold.
     """
 
     absolute_tolerance = 1e-2
     relative_tolerance = 1e-2
     max_steps = 16**4
-    solver = Tsit5()
-    parameters = SolverParameters(relative_tolerance, 
-                                  absolute_tolerance, 
-                                  step_size, 
-                                  time_interval, 
-                                  solver,
-                                  max_steps)
+    step_size = 0.01
+    solver = Heun()
+    parameters = SolverParameters(stepsize_controller=PIDController(rtol=relative_tolerance,
+                                                                    atol=absolute_tolerance),
+                                  step_size_internal=0.1,
+                                  step_size_output=step_size,
+                                  time_interval = time_interval,
+                                  solver=solver,
+                                  max_steps = max_steps)
 
-    U = system_sensitivity(vector_field, initial_condition, parameters)
+    U = system_sensitivity(vector_field, initial_condition, system_parameters, parameters)
     A = trapezoidal_correlation_weighted(U, step_size, kernel)
 
     return jnp.sqrt(abs(jnp.linalg.det(A)))
```

### Comparing `trajectory_manifold-0.0.1/trajectory_manifold/optimize.py` & `trajectory_manifold-0.0.2/trajectory_manifold/optimize.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,53 +2,67 @@
 
 This module contains useful functions for optimization on the
 trajectory manifold. It enables the computation of the pullback
 of gradients into the ambient space, as well as helper functions
 for grid-based methods.
 """
 from typing import Callable
-from jaxtyping import Float, Array, PyTree
+from jaxtyping import Float, Array
 import jax.numpy as jnp
 from jax import random
 from .manifold import system_sensitivity_and_solution, SolverParameters
-from .helpers import trapezoidal_matrix_product
+from .helpers import trapezoidal_matrix_product, trapezoidal_pytree_vector_product
 
 
 
 def distance_gradient(
     initial_condition: Float[Array, " dim"],
-    vector_field: Callable[[Float, Float[Array, " dim"], PyTree], Float[Array, " dim"]],
-    trajectory: Float[Array, " dim dim2"],
-    params: SolverParameters,
-) -> Float[Array, " dim"]:
+    system_params: Float[Array, " dim2"],
+    vector_field: Callable[[Float, Float[Array, " dim"], Float[Array, " dim2"]], Float[Array, " dim"]],
+    trajectory: Float[Array, " dim dim3"],
+    solver_params: SolverParameters,
+) -> tuple[Float[Array, " dim"], Float[Array, " dim2"]]:
     """Computes the gradient of the squared distance to a chosen trajectory.
     
     Computes the pullback along the transformation from initial conditions
     to system trajectories of the gradient of the squared distance from
     a given sampled trajectory in the ambient space.
 
     The gradient in the trajectory manifold is the projection of the gradient
     in the ambient space onto the tangent space of the manifold.
 
     Args:
         initial_condition: The initial condition around which to linearize.
         vector_field: Vector field defining the differential equation.
         trajectory: A sampled function from which the distance is computed.
-        params: Parameters for the ODE solvers.
+        solver_params: Parameters for the ODE solvers.
     
     Returns:
-        The gradient of the distance to a function"""
+        The gradient of the distance to a function
+    """
+
     sensitivity, solution = system_sensitivity_and_solution(vector_field,
                                                             initial_condition,
-                                                            params)
+                                                            system_params,
+                                                            solver_params)
     gradient_ambient = solution - trajectory
     gradient_statespace = trapezoidal_matrix_product(gradient_ambient[None, :, :], 
-                                                     sensitivity,
-                                                     params.step_size)
-    return gradient_statespace
+                                                     sensitivity[0],
+                                                     solver_params.step_size_output)
+
+    if isinstance(sensitivity[1], jnp.ndarray):
+        gradient_parameters = trapezoidal_matrix_product(gradient_ambient[None, :, :], 
+                                                         sensitivity[1],
+                                                         solver_params.step_size_output)
+    else:
+        gradient_parameters = trapezoidal_pytree_vector_product(gradient_ambient, 
+                                                                sensitivity[1],
+                                                                solver_params.step_size_output)
+
+    return gradient_statespace, gradient_parameters
     
 
 def zero_order_gradient_estimate(
     f: Callable[[Float[Array, " dim batch_size"]], Float[Array, " batch_size"]],
     x: Float[Array, " dim"],
     smoothing: float,
     batch_size: int,
```

### Comparing `trajectory_manifold-0.0.1/trajectory_manifold.egg-info/PKG-INFO` & `trajectory_manifold-0.0.2/trajectory_manifold.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajectory-manifold
-Version: 0.0.1
+Version: 0.0.2
 Summary: Statistically Rigorous ODE Forecasting
 Author-email: Helmuth Naumer <hnaumer2@illinois.edu>
 Project-URL: Homepage, https://github.com/helmuthn/trajectory_manifold
 Project-URL: Documentation, https://www.helmuthnaumer.com/trajectory_manifold/
 Project-URL: Bug Tracker, https://github.com/helmuthn/trajectory_manifold/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,7 +20,9 @@
 # Trajectory Manifold
 
 [![Documentation](https://img.shields.io/badge/Documentation-Main-darkgreen)](https://www.helmuthnaumer.com/trajectory_manifold/)
 
 This repository contains code around statistical estimation on the trajectory manifold.
 
 It is intended to accompany a paper currently under review.
+
+The directory `figures` contains code to reproduce the figures in the work, while the directory `examples` contains the quick start example from the documentation.
```

