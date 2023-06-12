# Comparing `tmp/upkie-0.5.0.tar.gz` & `tmp/upkie-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upkie-0.5.0.tar", last modified: Tue Jun  6 13:14:50 2023, max compression
+gzip compressed data, was "upkie-1.0.0.tar", last modified: Mon Jun 12 17:39:45 2023, max compression
```

## Comparing `upkie-0.5.0.tar` & `upkie-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     6760 2023-06-06 13:14:50.113429 upkie-0.5.0/README.md
--rw-r--r--   0        0        0     1909 2023-06-06 13:14:50.113429 upkie-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      695 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/__init__.py
--rw-r--r--   0        0        0     1041 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/BUILD
--rw-r--r--   0        0        0     1214 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/__init__.py
--rw-r--r--   0        0        0     2809 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/standing_reward.py
--rw-r--r--   0        0        0      549 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/tests/BUILD
--rw-r--r--   0        0        0     2482 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/tests/upkie_base_env_test.py
--rw-r--r--   0        0        0     2372 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/tests/upkie_servos_env_test.py
--rw-r--r--   0        0        0     2256 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/tests/upkie_wheels_env_test.py
--rw-r--r--   0        0        0     6197 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/upkie_base_env.py
--rw-r--r--   0        0        0     7149 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/upkie_servos_env.py
--rw-r--r--   0        0        0     6049 2023-06-06 13:14:50.089423 upkie-0.5.0/upkie/envs/upkie_wheels_env.py
--rw-r--r--   0        0        0      327 2023-06-06 13:14:50.101426 upkie-0.5.0/upkie/observers/base_pitch/BUILD
--rw-r--r--   0        0        0      822 2023-06-06 13:14:50.101426 upkie-0.5.0/upkie/observers/base_pitch/__init__.py
--rw-r--r--   0        0        0     4550 2023-06-06 13:14:50.101426 upkie-0.5.0/upkie/observers/base_pitch/base_pitch.py
--rw-r--r--   0        0        0      305 2023-06-06 13:14:50.101426 upkie-0.5.0/upkie/observers/base_pitch/tests/BUILD
--rw-r--r--   0        0        0     2483 2023-06-06 13:14:50.101426 upkie-0.5.0/upkie/observers/base_pitch/tests/base_pitch_test.py
--rw-r--r--   0        0        0      624 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/utils/BUILD
--rw-r--r--   0        0        0     1896 2023-06-06 13:14:50.105427 upkie-0.5.0/upkie/utils/clamp.py
--rw-r--r--   0        0        0      803 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/utils/exceptions.py
--rw-r--r--   0        0        0     2820 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/utils/filters.py
--rw-r--r--   0        0        0     2433 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/utils/pinocchio.py
--rw-r--r--   0        0        0     1231 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/utils/realtime.py
--rw-r--r--   0        0        0     1983 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/utils/spdlog.py
--rw-r--r--   0        0        0      453 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/utils/tests/BUILD
--rw-r--r--   0        0        0     1303 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/utils/tests/clamp_test.py
--rw-r--r--   0        0        0     2232 2023-06-06 13:14:50.109428 upkie-0.5.0/upkie/utils/tests/pinocchio_test.py
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 upkie-0.5.0/setup.py
--rw-r--r--   0        0        0     8221 1970-01-01 00:00:00.000000 upkie-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     6671 2023-06-12 17:39:45.135682 upkie-1.0.0/README.md
+-rw-r--r--   0        0        0     1909 2023-06-12 17:39:45.135682 upkie-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/__init__.py
+-rw-r--r--   0        0        0     1084 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/BUILD
+-rw-r--r--   0        0        0     1236 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/__init__.py
+-rw-r--r--   0        0        0     2809 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/standing_reward.py
+-rw-r--r--   0        0        0      549 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/tests/BUILD
+-rw-r--r--   0        0        0     2530 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/tests/upkie_base_env_test.py
+-rw-r--r--   0        0        0     2446 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/tests/upkie_servos_env_test.py
+-rw-r--r--   0        0        0     2330 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/tests/upkie_wheels_env_test.py
+-rw-r--r--   0        0        0     8063 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/upkie_base_env.py
+-rw-r--r--   0        0        0     7363 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/upkie_servos_env.py
+-rw-r--r--   0        0        0     6263 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/upkie_wheels_env.py
+-rw-r--r--   0        0        0      327 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/BUILD
+-rw-r--r--   0        0        0      822 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/__init__.py
+-rw-r--r--   0        0        0     4550 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/base_pitch.py
+-rw-r--r--   0        0        0      305 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/tests/BUILD
+-rw-r--r--   0        0        0     2483 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/tests/base_pitch_test.py
+-rw-r--r--   0        0        0      694 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/BUILD
+-rw-r--r--   0        0        0     1896 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/clamp.py
+-rw-r--r--   0        0        0      803 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/exceptions.py
+-rw-r--r--   0        0        0     2820 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/filters.py
+-rw-r--r--   0        0        0     2433 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/pinocchio.py
+-rw-r--r--   0        0        0     1231 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/realtime.py
+-rw-r--r--   0        0        0     1983 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/spdlog.py
+-rw-r--r--   0        0        0      453 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/tests/BUILD
+-rw-r--r--   0        0        0     1303 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/tests/clamp_test.py
+-rw-r--r--   0        0        0     2232 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/tests/pinocchio_test.py
+-rw-r--r--   0        0        0     8132 1970-01-01 00:00:00.000000 upkie-1.0.0/PKG-INFO
```

### Comparing `upkie-0.5.0/README.md` & `upkie-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Upkie wheeled biped
 
 [![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/upkie/bazel.yml?branch=main)](https://github.com/tasts-robots/upkie/actions/workflows/bazel.yml)
 [![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://tasts-robots.org/doc/upkie/)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/upkie/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/upkie?branch=main)
-[![Vulp](https://img.shields.io/badge/%F0%9F%A6%8A%20vulp-1.1.1-orange)](https://github.com/tasts-robots/vulp)
+[![Vulp](https://img.shields.io/badge/%F0%9F%A6%8A%20vulp-1.2.0-orange)](https://github.com/tasts-robots/vulp)
 [![Chat](https://img.shields.io/badge/matrix-joint%20chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
 Main repository to build and control **Upkie** wheeled bipeds. Made for Linux 🐧
 
 Questions about using the code, contributing, or balancing robots in general are welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://github.com/tasts-robots/upkie/discussions).
 
 ## Quick test
@@ -24,30 +24,27 @@
 
 Connect a USB controller to move the robot around 🎮
 
 ## Example
 
 ```python
 import gym
-import loop_rate_limiters
 import upkie.envs
 
 upkie.envs.register()
 
-with gym.make("UpkieWheelsEnv-v2") as env:
+with gym.make("UpkieWheelsEnv-v2", frequency=200.0) as env:
     observation = env.reset()
     action = 0.0 * env.action_space.sample()
-    rate = loop_rate_limiters.RateLimiter(frequency=200.0)
     for step in range(1_000_000):
         observation, reward, done, _ = env.step(action)
         if done:
             observation = env.reset()
         pitch = observation[0]
         action[0] = 10.0 * pitch
-        rate.sleep()
 ```
 
 ## Installation
 
 ### PyPI
 
 [![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
 # Upkie wheeled biped [![Build](https://img.shields.io/github/actions/workflow/
 status/tasts-robots/upkie/bazel.yml?branch=main)](https://github.com/tasts-
 robots/upkie/actions/workflows/bazel.yml) [![Documentation](https://
 img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)]
 (https://tasts-robots.org/doc/upkie/) [![Coverage](https://coveralls.io/repos/
 github/tasts-robots/upkie/badge.svg?branch=main)](https://coveralls.io/github/
 tasts-robots/upkie?branch=main) [![Vulp](https://img.shields.io/badge/
-%F0%9F%A6%8A%20vulp-1.1.1-orange)](https://github.com/tasts-robots/vulp) [!
+%F0%9F%A6%8A%20vulp-1.2.0-orange)](https://github.com/tasts-robots/vulp) [!
 [Chat](https://img.shields.io/badge/matrix-joint%20chat-%234eb899)](https://
 app.element.io/#/room/#tasts-robots:matrix.org) Main repository to build and
 control **Upkie** wheeled bipeds. Made for Linux ð§ Questions about using the
 code, contributing, or balancing robots in general are welcome in the
 [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on
 the [Chat](https://github.com/tasts-robots/upkie/discussions). ## Quick test
 Run a simulated Upkie right away from the command line, no installation
 required: [https://user-images.githubusercontent.com/1189580/170496331-
 e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png] ```console $ git clone https://
 github.com/tasts-robots/upkie.git $ cd upkie $ ./start_test_balancer.sh ```
 Connect a USB controller to move the robot around ð® ## Example ```python
-import gym import loop_rate_limiters import upkie.envs upkie.envs.register()
-with gym.make("UpkieWheelsEnv-v2") as env: observation = env.reset() action =
-0.0 * env.action_space.sample() rate = loop_rate_limiters.RateLimiter
-(frequency=200.0) for step in range(1_000_000): observation, reward, done, _ =
-env.step(action) if done: observation = env.reset() pitch = observation[0]
-action[0] = 10.0 * pitch rate.sleep() ``` ## Installation ### PyPI [![PyPI
+import gym import upkie.envs upkie.envs.register() with gym.make
+("UpkieWheelsEnv-v2", frequency=200.0) as env: observation = env.reset() action
+= 0.0 * env.action_space.sample() for step in range(1_000_000): observation,
+reward, done, _ = env.step(action) if done: observation = env.reset() pitch =
+observation[0] action[0] = 10.0 * pitch ``` ## Installation ### PyPI [![PyPI
 version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/
 ) [![PyPI downloads](https://pepy.tech/badge/upkie/month)](https://pepy.tech/
 project/upkie) ```console $ pip install upkie ``` ## Code overview This
 repository uses [Bazel](https://bazel.build/) for building and testing. One
 benefit of this choice is that there is no dependency to install: Bazel builds
 everything locally in a local cache. Compilation will only take a while the
 first time. Locomotion code is organized into *spines*, which communicate with
```

### Comparing `upkie-0.5.0/pyproject.toml` & `upkie-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/__init__.py` & `upkie-1.0.0/upkie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python module to control Upkie wheeled bipeds."""
 
-__version__ = "0.5.0"
+__version__ = "1.0.0"
```

### Comparing `upkie-0.5.0/upkie/envs/BUILD` & `upkie-1.0.0/upkie/envs/BUILD`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         "standing_reward.py",
         "upkie_base_env.py",
     ],
     deps = [
         "@upkie//observers/base_pitch",
         "@vulp//spine:python",
         requirement("gym"),
+        requirement("loop_rate_limiters"),
         requirement("pyyaml"),
         requirement("upkie_description"),
     ],
 )
 
 py_library(
     name = "upkie_wheels_env",
```

### Comparing `upkie-0.5.0/upkie/envs/__init__.py` & `upkie-1.0.0/upkie/envs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,10 +33,11 @@
         entry_point="upkie.envs:UpkieWheelsEnv",
         max_episode_steps=1_000_000_000,
     )
 
 
 __all__ = [
     "UpkieBaseEnv",
+    "UpkieServosEnv",
     "UpkieWheelsEnv",
     "register",
 ]
```

### Comparing `upkie-0.5.0/upkie/envs/standing_reward.py` & `upkie-1.0.0/upkie/envs/standing_reward.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/envs/tests/BUILD` & `upkie-1.0.0/upkie/envs/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/envs/tests/upkie_base_env_test.py` & `upkie-1.0.0/upkie/envs/tests/upkie_base_env_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """Test UpkieBaseEnv."""
 
 import unittest
 
 import numpy as np
 import posix_ipc
 
-from upkie.envs import UpkieBaseEnv
+from envs import UpkieBaseEnv
 
 
 class MockSpine:
     def __init__(self):
         self.observation = {
             "number": 0,
             "servo": {
@@ -72,15 +72,18 @@
 class TestUpkieBaseEnv(unittest.TestCase):
     def setUp(self):
         shm_name = "/vroum"
         shared_memory = posix_ipc.SharedMemory(
             shm_name, posix_ipc.O_RDWR | posix_ipc.O_CREAT, size=42
         )
         self.env = UpkieBaseChild(
-            config=None, fall_pitch=1.0, shm_name=shm_name
+            config=None,
+            fall_pitch=1.0,
+            frequency=100.0,
+            shm_name=shm_name,
         )
         shared_memory.close_fd()
         self.env._spine = MockSpine()
 
     def test_reset(self):
         _, observation_dict = self.env.reset(return_info=True)
         self.assertGreaterEqual(observation_dict["number"], 1)
```

### Comparing `upkie-0.5.0/upkie/envs/tests/upkie_servos_env_test.py` & `upkie-1.0.0/upkie/envs/tests/upkie_servos_env_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """Tests for UpkieServosEnv."""
 
 import unittest
 
 import numpy as np
 import posix_ipc
 
-from upkie.envs import UpkieServosEnv
+from envs import UpkieServosEnv
 
 
 class MockSpine:
     def __init__(self):
         self.observation = {
             "number": 0,
             "servo": {
@@ -64,15 +64,19 @@
 
 class TestUpkieServosEnv(unittest.TestCase):
     def setUp(self):
         shm_name = "/vroum"
         shared_memory = posix_ipc.SharedMemory(
             shm_name, posix_ipc.O_RDWR | posix_ipc.O_CREAT, size=42
         )
-        self.env = UpkieServosEnv(shm_name=shm_name)
+        self.env = UpkieServosEnv(
+            fall_pitch=1.0,
+            frequency=100.0,
+            shm_name=shm_name,
+        )
         shared_memory.close_fd()
         self.env._spine = MockSpine()
 
     def test_reset(self):
         observation, observation_dict = self.env.reset(return_info=True)
         self.assertAlmostEqual(
             observation[1], observation_dict["wheel_odometry"]["position"]
```

### Comparing `upkie-0.5.0/upkie/envs/tests/upkie_wheels_env_test.py` & `upkie-1.0.0/upkie/envs/tests/upkie_wheels_env_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """Test UpkieWheelsEnv."""
 
 import unittest
 
 import numpy as np
 import posix_ipc
 
-from upkie.envs import UpkieWheelsEnv
+from envs import UpkieWheelsEnv
 
 
 class MockSpine:
     def __init__(self):
         self.observation = {
             "number": 0,
             "servo": {
@@ -60,15 +60,19 @@
 
 class TestUpkieWheelsEnv(unittest.TestCase):
     def setUp(self):
         shm_name = "/vroum"
         shared_memory = posix_ipc.SharedMemory(
             shm_name, posix_ipc.O_RDWR | posix_ipc.O_CREAT, size=42
         )
-        self.env = UpkieWheelsEnv(shm_name=shm_name)
+        self.env = UpkieWheelsEnv(
+            fall_pitch=1.0,
+            frequency=100.0,
+            shm_name=shm_name,
+        )
         shared_memory.close_fd()
         self.env._spine = MockSpine()
 
     def test_reset(self):
         observation, observation_dict = self.env.reset(return_info=True)
         self.assertAlmostEqual(
             observation[1], observation_dict["wheel_odometry"]["position"]
```

### Comparing `upkie-0.5.0/upkie/envs/upkie_base_env.py` & `upkie-1.0.0/upkie/envs/upkie_base_env.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
+import asyncio
 from typing import Dict, Optional, Tuple, Union
 
 import gym
 import numpy as np
+from loop_rate_limiters import AsyncRateLimiter, RateLimiter
 from vulp.spine import SpineInterface
 
 from upkie.observers.base_pitch import compute_base_pitch_from_imu
 
 DEFAULT_CONFIG = {
     "bullet": {
         "control_mode": "torque",
@@ -50,33 +52,39 @@
 
     @note This environment is made to run on a single CPU thread rather than on
     GPU/TPU. The downside for reinforcement learning is that computations are
     not massively parallel. The upside is that it simplifies deployment to the
     real robot, as it relies on the same spine interface that runs on Upkie.
     """
 
+    __frequency: float
+    __async_rate: Optional[AsyncRateLimiter]
+    __rate: Optional[RateLimiter]
     _spine: SpineInterface
     config: dict
     fall_pitch: float
 
     def __init__(
         self,
-        config: dict,
+        config: Optional[dict],
         fall_pitch: float,
+        frequency: float,
         shm_name: str,
     ) -> None:
         """!
         Initialize environment.
 
         @param config Configuration dictionary, also sent to the spine.
         @param fall_pitch Fall pitch angle, in radians.
+        @param frequency Regulated frequency of the control loop, in Hz.
         @param shm_name Name of shared-memory file.
         """
         if config is None:
             config = DEFAULT_CONFIG
+        self.__frequency = frequency
         self._spine = SpineInterface(shm_name)
         self.config = config
         self.fall_pitch = fall_pitch
 
     def close(self) -> None:
         """!
         Stop the spine properly.
@@ -99,63 +107,100 @@
         @param options Currently unused.
         @returns
             - ``observation``: the initial vectorized observation.
             - ``info``: an optional dictionary containing extra information.
                 It is only returned if ``return_info`` is set to true.
         """
         # super().reset(seed=seed)  # we are pinned at gym==0.21.0
+        self.__reset_rates()
         self._spine.stop()
         self._spine.start(self.config)
         self._spine.get_observation()  # might be a pre-reset observation
         observation_dict = self._spine.get_observation()
         self.parse_first_observation(observation_dict)
         observation = self.vectorize_observation(observation_dict)
         if not return_info:
             return observation
         else:  # return_info
             return observation, observation_dict
 
+    def __reset_rates(self):
+        self.__async_rate = None
+        self.__rate = None
+        try:
+            asyncio.get_running_loop()
+            self.__async_rate = AsyncRateLimiter(self.__frequency)
+        except RuntimeError:  # not asyncio
+            self.__rate = RateLimiter(self.__frequency)
+
     def step(self, action: np.ndarray) -> Tuple[np.ndarray, float, bool, dict]:
         """!
-        Run one timestep of the environment's dynamics. When end of episode is
-        reached, you are responsible for calling `reset()` to reset the
-        environment's state.
+        Run one timestep of the environment's dynamics. When the end of the
+        episode is reached, you are responsible for calling `reset()` to reset
+        the environment's state.
 
         @param action Action from the agent.
         @returns
             - ``observation``: Agent's observation of the environment.
             - ``reward``: Amount of reward returned after previous action.
             - ``done``: Whether the agent reaches the terminal state, which can
               be a good or a bad thing. If true, the user needs to call
               :func:`reset()`.
             - ``info``: Contains auxiliary diagnostic information (helpful for
               debugging, logging, and sometimes learning).
         """
         action_dict = self.dictionarize_action(action)
+        self.__rate.sleep()  # wait until clock tick to send the action
+        return self.__step(action_dict)
+
+    async def async_step(
+        self, action: np.ndarray
+    ) -> Tuple[np.ndarray, float, bool, dict]:
+        """!
+        Run one timestep of the environment's dynamics using asynchronous I/O.
+        When the end of the episode is reached, you are responsible for calling
+        `reset()` to reset the environment's state.
+
+        @param action Action from the agent.
+        @returns
+            - ``observation``: Agent's observation of the environment.
+            - ``reward``: Amount of reward returned after previous action.
+            - ``done``: Whether the agent reaches the terminal state, which can
+              be a good or a bad thing. If true, the user needs to call
+              :func:`reset()`.
+            - ``info``: Contains auxiliary diagnostic information (helpful for
+              debugging, logging, and sometimes learning).
+        """
+        action_dict = self.dictionarize_action(action)
+        await self.__async_rate.sleep()  # send action at next clock tick
+        return self.__step(action_dict)
+
+    def __step(
+        self, action_dict: dict
+    ) -> Tuple[np.ndarray, float, bool, dict]:
         self._spine.set_action(action_dict)
         observation_dict = self._spine.get_observation()
-        imu = observation_dict["imu"]
-        # TODO(scaron): use tilt (angle to the vertical) rather than pitch
-        pitch = compute_base_pitch_from_imu(imu["orientation"])
         observation = self.vectorize_observation(observation_dict)
         reward = self.reward.get(observation)
-        done = self.detect_fall(pitch)
+        done = self.detect_fall(observation_dict)
         info = {
             "action": action_dict,
             "observation": observation_dict,
         }
         return observation, reward, done, info
 
-    def detect_fall(self, pitch: float) -> bool:
+    def detect_fall(self, observation_dict: dict) -> bool:
         """!
         Detect a fall based on the body-to-world pitch angle.
 
         @param pitch Current pitch angle in [rad].
         @returns True if and only if a fall is detected.
         """
+        imu = observation_dict["imu"]
+        pitch = compute_base_pitch_from_imu(imu["orientation"])
         return abs(pitch) > self.fall_pitch
 
     @abc.abstractmethod
     def parse_first_observation(self, observation_dict: dict) -> None:
         """!
         Parse first observation after the spine interface is initialize.
```

### Comparing `upkie-0.5.0/upkie/envs/upkie_servos_env.py` & `upkie-1.0.0/upkie/envs/upkie_servos_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,30 +93,37 @@
 
     See also @ref envs.upkie_base_env.UpkieBaseEnv "UpkieBaseEnv" for notes on
     using this environment.
     """
 
     reward: StandingReward
     robot: pin.RobotWrapper
-    version: int = 1
+    version: int = 2
 
     def __init__(
         self,
         config: Optional[dict] = None,
         fall_pitch: float = 1.0,
+        frequency: float = 200.0,
         shm_name: str = "/vulp",
     ):
         """!
         Initialize environment.
 
         @param config Configuration dictionary, also sent to the spine.
         @param fall_pitch Fall pitch angle, in radians.
+        @param frequency Regulated frequency of the control loop, in Hz.
         @param shm_name Name of shared-memory file.
         """
-        super().__init__(config, fall_pitch, shm_name)
+        super().__init__(
+            config=config,
+            fall_pitch=fall_pitch,
+            frequency=frequency,
+            shm_name=shm_name,
+        )
 
         robot = upkie_description.load_in_pinocchio(root_joint=None)
         model = robot.model
 
         q_min, q_max = box_position_limits(model)
         v_max = box_velocity_limits(model)
         tau_max = box_torque_limits(model)
```

### Comparing `upkie-0.5.0/upkie/envs/upkie_wheels_env.py` & `upkie-1.0.0/upkie/envs/upkie_wheels_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 from typing import Optional
 
 import numpy as np
-
 from gym import spaces
+
 from upkie.observers.base_pitch import compute_base_pitch_from_imu
 
 from .standing_reward import StandingReward
 from .upkie_base_env import UpkieBaseEnv
 
 MAX_BASE_PITCH: float = np.pi
 MAX_GROUND_POSITION: float = float("inf")
@@ -75,41 +75,48 @@
 
     See also @ref envs.upkie_base_env.UpkieBaseEnv "UpkieBaseEnv" for notes on
     using this environment.
     """
 
     fall_pitch: float
     max_ground_velocity: float
-    version: int = 2
+    version: int = 3
     wheel_radius: float
 
     LEG_JOINTS = [
         f"{side}_{joint}"
         for side in ("left", "right")
         for joint in ("hip", "knee")
     ]
 
     def __init__(
         self,
         config: Optional[dict] = None,
         fall_pitch: float = 1.0,
+        frequency: float = 200.0,
         max_ground_velocity: float = 1.0,
         shm_name: str = "/vulp",
         wheel_radius: float = 0.06,
     ):
         """!
         Initialize environment.
 
         @param config Configuration dictionary, also sent to the spine.
         @param fall_pitch Fall pitch angle, in radians.
+        @param frequency Regulated frequency of the control loop, in Hz.
         @param max_ground_velocity Maximum commanded ground velocity in m/s.
         @param shm_name Name of shared-memory file.
         @param wheel_radius Wheel radius in [m].
         """
-        super().__init__(config, fall_pitch, shm_name)
+        super().__init__(
+            config=config,
+            fall_pitch=fall_pitch,
+            frequency=frequency,
+            shm_name=shm_name,
+        )
 
         observation_limit = np.array(
             [
                 MAX_BASE_PITCH,
                 MAX_GROUND_POSITION,
                 max_ground_velocity,
                 MAX_IMU_ANGULAR_VELOCITY,
```

### Comparing `upkie-0.5.0/upkie/observers/base_pitch/__init__.py` & `upkie-1.0.0/upkie/observers/base_pitch/__init__.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/observers/base_pitch/base_pitch.py` & `upkie-1.0.0/upkie/observers/base_pitch/base_pitch.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/observers/base_pitch/tests/base_pitch_test.py` & `upkie-1.0.0/upkie/observers/base_pitch/tests/base_pitch_test.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/utils/BUILD` & `upkie-1.0.0/upkie/utils/BUILD`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     srcs = ["clamp.py"],
     deps = [
         ":spdlog",
     ],
 )
 
 py_library(
+    name = "exceptions",
+    srcs = ["exceptions.py"],
+)
+
+py_library(
     name = "filters",
     srcs = ["filters.py"],
     deps = [
         ":clamp",
     ],
 )
```

### Comparing `upkie-0.5.0/upkie/utils/clamp.py` & `upkie-1.0.0/upkie/utils/clamp.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/utils/exceptions.py` & `upkie-1.0.0/upkie/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/utils/filters.py` & `upkie-1.0.0/upkie/utils/filters.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/utils/pinocchio.py` & `upkie-1.0.0/upkie/utils/pinocchio.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/utils/realtime.py` & `upkie-1.0.0/upkie/utils/realtime.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/utils/spdlog.py` & `upkie-1.0.0/upkie/utils/spdlog.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/utils/tests/clamp_test.py` & `upkie-1.0.0/upkie/utils/tests/clamp_test.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/upkie/utils/tests/pinocchio_test.py` & `upkie-1.0.0/upkie/utils/tests/pinocchio_test.py`

 * *Files identical despite different names*

### Comparing `upkie-0.5.0/PKG-INFO` & `upkie-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upkie
-Version: 0.5.0
+Version: 1.0.0
 Summary: Python module to control Upkie wheeled bipeds.
 Keywords: wheeled,biped,robot,balance,motion,control,robotics
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,15 @@
 Project-URL: Tracker, https://github.com/tasts-robots/upkie/issues
 
 # Upkie wheeled biped
 
 [![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/upkie/bazel.yml?branch=main)](https://github.com/tasts-robots/upkie/actions/workflows/bazel.yml)
 [![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://tasts-robots.org/doc/upkie/)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/upkie/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/upkie?branch=main)
-[![Vulp](https://img.shields.io/badge/%F0%9F%A6%8A%20vulp-1.1.1-orange)](https://github.com/tasts-robots/vulp)
+[![Vulp](https://img.shields.io/badge/%F0%9F%A6%8A%20vulp-1.2.0-orange)](https://github.com/tasts-robots/vulp)
 [![Chat](https://img.shields.io/badge/matrix-joint%20chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
 Main repository to build and control **Upkie** wheeled bipeds. Made for Linux 🐧
 
 Questions about using the code, contributing, or balancing robots in general are welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://github.com/tasts-robots/upkie/discussions).
 
 ## Quick test
@@ -57,30 +57,27 @@
 
 Connect a USB controller to move the robot around 🎮
 
 ## Example
 
 ```python
 import gym
-import loop_rate_limiters
 import upkie.envs
 
 upkie.envs.register()
 
-with gym.make("UpkieWheelsEnv-v2") as env:
+with gym.make("UpkieWheelsEnv-v2", frequency=200.0) as env:
     observation = env.reset()
     action = 0.0 * env.action_space.sample()
-    rate = loop_rate_limiters.RateLimiter(frequency=200.0)
     for step in range(1_000_000):
         observation, reward, done, _ = env.step(action)
         if done:
             observation = env.reset()
         pitch = observation[0]
         action[0] = 10.0 * pitch
-        rate.sleep()
 ```
 
 ## Installation
 
 ### PyPI
 
 [![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
```

