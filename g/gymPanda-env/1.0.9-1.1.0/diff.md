# Comparing `tmp/gymPanda_env-1.0.9-py3-none-any.whl.zip` & `tmp/gymPanda_env-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3386 bytes, number of entries: 7
+Zip file size: 3434 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx      128 b- defN 23-Jun-07 18:48 gym_panda_env/__init__.py
 -rw-rw-r--  2.0 unx       52 b- defN 23-Jun-07 18:46 gym_panda_env/envs/__init__.py
--rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-07 19:32 gym_panda_env/envs/panda_env.py
--rw-rw-r--  2.0 unx      238 b- defN 23-Jun-07 19:32 gymPanda_env-1.0.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 19:32 gymPanda_env-1.0.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jun-07 19:32 gymPanda_env-1.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      571 b- defN 23-Jun-07 19:32 gymPanda_env-1.0.9.dist-info/RECORD
-7 files, 5878 bytes uncompressed, 2364 bytes compressed:  59.8%
+-rw-rw-r--  2.0 unx     4948 b- defN 23-Jun-12 17:00 gym_panda_env/envs/panda_env.py
+-rw-rw-r--  2.0 unx      238 b- defN 23-Jun-12 17:01 gymPanda_env-1.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 17:01 gymPanda_env-1.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jun-12 17:01 gymPanda_env-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      571 b- defN 23-Jun-12 17:01 gymPanda_env-1.1.0.dist-info/RECORD
+7 files, 6043 bytes uncompressed, 2412 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: gym_panda_env/envs/__init__.py
 Comment: 
 
 Filename: gym_panda_env/envs/panda_env.py
 Comment: 
 
-Filename: gymPanda_env-1.0.9.dist-info/METADATA
+Filename: gymPanda_env-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: gymPanda_env-1.0.9.dist-info/WHEEL
+Filename: gymPanda_env-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: gymPanda_env-1.0.9.dist-info/top_level.txt
+Filename: gymPanda_env-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gymPanda_env-1.0.9.dist-info/RECORD
+Filename: gymPanda_env-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_panda_env/envs/panda_env.py

```diff
@@ -49,15 +49,15 @@
             done = False
 
         info = {'object_position': state_object}
         observation = state_robot + state_fingers
 
         return observation, reward, done, info
 
-    def reset(self):
+    def reset(self,seed=None, option=None):
         p.resetSimulation()
         p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,0) # we will enable rendering after we loaded everything
         p.setGravity(0,0,-10)
         urdfRootPath=pybullet_data.getDataPath()
 
         tableUid = p.loadURDF(os.path.join(urdfRootPath, "table/table.urdf"),basePosition=[0.5,0,-0.65])
         trayUid = p.loadURDF(os.path.join(urdfRootPath, "tray/traybox.urdf"),basePosition=[0.65,0,0])
@@ -72,16 +72,23 @@
         state_object= [random.uniform(0.5,0.8),random.uniform(-0.2,0.2),0.05]
         self.objectUid = p.loadURDF(os.path.join(urdfRootPath, "random_urdfs/000/000.urdf"), basePosition=state_object)
 
         state_robot = p.getLinkState(self.pandaUid, 11)[0]
         state_fingers = (p.getJointState(self.pandaUid,9)[0], p.getJointState(self.pandaUid, 10)[0])
 
         self.observation = state_robot + state_fingers
+        
         p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,1) # rendering's back on again
-        return np.array(self.observation).astype(np.float32)
+
+
+        observation = np.array(self.observation).astype(np.float32)
+        info = {"None" : None}
+
+        return observation, info
+
 
     def render(self, mode='human'):
         view_matrix = p.computeViewMatrixFromYawPitchRoll(cameraTargetPosition=[0.7,0,0.05],
                                                             distance=.7,
                                                             yaw=90,
                                                             pitch=-70,
                                                             roll=0,
@@ -98,10 +105,12 @@
 
         rgb_array = np.array(px, dtype=np.uint8)
         rgb_array = np.reshape(rgb_array, (720,960, 4))
 
         rgb_array = rgb_array[:, :, :3]
         return rgb_array
 
+    def _get_state(self):
+        return self.observation
 
     def close(self):
         p.disconnect()
```

