# Comparing `tmp/gymPanda_env-1.1.1-py3-none-any.whl.zip` & `tmp/gymPanda_env-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3443 bytes, number of entries: 7
+Zip file size: 3430 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx      128 b- defN 23-Jun-07 18:48 gym_panda_env/__init__.py
 -rw-rw-r--  2.0 unx       52 b- defN 23-Jun-07 18:46 gym_panda_env/envs/__init__.py
--rw-rw-r--  2.0 unx     5038 b- defN 23-Jun-12 17:04 gym_panda_env/envs/panda_env.py
--rw-rw-r--  2.0 unx      238 b- defN 23-Jun-12 17:04 gymPanda_env-1.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 17:04 gymPanda_env-1.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jun-12 17:04 gymPanda_env-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      571 b- defN 23-Jun-12 17:04 gymPanda_env-1.1.1.dist-info/RECORD
-7 files, 6133 bytes uncompressed, 2421 bytes compressed:  60.5%
+-rw-rw-r--  2.0 unx     5017 b- defN 23-Jun-12 17:06 gym_panda_env/envs/panda_env.py
+-rw-rw-r--  2.0 unx      238 b- defN 23-Jun-12 17:06 gymPanda_env-1.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 17:06 gymPanda_env-1.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jun-12 17:06 gymPanda_env-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      571 b- defN 23-Jun-12 17:06 gymPanda_env-1.1.2.dist-info/RECORD
+7 files, 6112 bytes uncompressed, 2408 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: gym_panda_env/envs/__init__.py
 Comment: 
 
 Filename: gym_panda_env/envs/panda_env.py
 Comment: 
 
-Filename: gymPanda_env-1.1.1.dist-info/METADATA
+Filename: gymPanda_env-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: gymPanda_env-1.1.1.dist-info/WHEEL
+Filename: gymPanda_env-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: gymPanda_env-1.1.1.dist-info/top_level.txt
+Filename: gymPanda_env-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gymPanda_env-1.1.1.dist-info/RECORD
+Filename: gymPanda_env-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_panda_env/envs/panda_env.py

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import random
 
 class PandaGymEnv(gym.Env):
     metadata = {'render.modes': ['human']}
 
     def __init__(self):
-        p.connect(p.GUI, options="--opengl2") #Connects to GUI
+        p.connect(p.GUI) #Connects to GUI
         p.resetDebugVisualizerCamera(cameraDistance=1.5, cameraYaw=0, cameraPitch=-40, cameraTargetPosition=[0.55,-0.35,0.2]) # Set convinient camera pose
         self.action_space = spaces.Box(np.array([-1]*4), np.array([1]*4)) # Define continuous action space without fingers orientation here
         self.observation_space = spaces.Box(np.array([-1]*5), np.array([1]*5)) # Define observation space 
 
     def step(self, action):
         p.configureDebugVisualizer(p.COV_ENABLE_SINGLE_STEP_RENDERING) #Smooth display
         orientation = p.getQuaternionFromEuler([0.,-math.pi,math.pi/2.])
```

