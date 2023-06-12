# Comparing `tmp/gymPanda_env-1.1.0-py3-none-any.whl.zip` & `tmp/gymPanda_env-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3434 bytes, number of entries: 7
+Zip file size: 3443 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx      128 b- defN 23-Jun-07 18:48 gym_panda_env/__init__.py
 -rw-rw-r--  2.0 unx       52 b- defN 23-Jun-07 18:46 gym_panda_env/envs/__init__.py
--rw-rw-r--  2.0 unx     4948 b- defN 23-Jun-12 17:00 gym_panda_env/envs/panda_env.py
--rw-rw-r--  2.0 unx      238 b- defN 23-Jun-12 17:01 gymPanda_env-1.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 17:01 gymPanda_env-1.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jun-12 17:01 gymPanda_env-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      571 b- defN 23-Jun-12 17:01 gymPanda_env-1.1.0.dist-info/RECORD
-7 files, 6043 bytes uncompressed, 2412 bytes compressed:  60.1%
+-rw-rw-r--  2.0 unx     5038 b- defN 23-Jun-12 17:04 gym_panda_env/envs/panda_env.py
+-rw-rw-r--  2.0 unx      238 b- defN 23-Jun-12 17:04 gymPanda_env-1.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 17:04 gymPanda_env-1.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jun-12 17:04 gymPanda_env-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      571 b- defN 23-Jun-12 17:04 gymPanda_env-1.1.1.dist-info/RECORD
+7 files, 6133 bytes uncompressed, 2421 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: gym_panda_env/envs/__init__.py
 Comment: 
 
 Filename: gym_panda_env/envs/panda_env.py
 Comment: 
 
-Filename: gymPanda_env-1.1.0.dist-info/METADATA
+Filename: gymPanda_env-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: gymPanda_env-1.1.0.dist-info/WHEEL
+Filename: gymPanda_env-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: gymPanda_env-1.1.0.dist-info/top_level.txt
+Filename: gymPanda_env-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gymPanda_env-1.1.0.dist-info/RECORD
+Filename: gymPanda_env-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_panda_env/envs/panda_env.py

```diff
@@ -50,39 +50,38 @@
 
         info = {'object_position': state_object}
         observation = state_robot + state_fingers
 
         return observation, reward, done, info
 
     def reset(self,seed=None, option=None):
+        self.step_counter = 0
         p.resetSimulation()
         p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,0) # we will enable rendering after we loaded everything
-        p.setGravity(0,0,-10)
         urdfRootPath=pybullet_data.getDataPath()
+        p.setGravity(0,0,-10)
 
-        tableUid = p.loadURDF(os.path.join(urdfRootPath, "table/table.urdf"),basePosition=[0.5,0,-0.65])
-        trayUid = p.loadURDF(os.path.join(urdfRootPath, "tray/traybox.urdf"),basePosition=[0.65,0,0])
         planeUid = p.loadURDF(os.path.join(urdfRootPath,"plane.urdf"), basePosition=[0,0,-0.65])
-        self.pandaUid = p.loadURDF(os.path.join(urdfRootPath, "franka_panda/panda.urdf"),useFixedBase=True)
-
 
         rest_poses = [0,-0.215,0,-2.57,0,2.356,2.356,0.08,0.08]
+        self.pandaUid = p.loadURDF(os.path.join(urdfRootPath, "franka_panda/panda.urdf"),useFixedBase=True)
         for i in range(7):
             p.resetJointState(self.pandaUid,i, rest_poses[i])
+        p.resetJointState(self.pandaUid, 9, 0.08)
+        p.resetJointState(self.pandaUid,10, 0.08)
+        tableUid = p.loadURDF(os.path.join(urdfRootPath, "table/table.urdf"),basePosition=[0.5,0,-0.65])
+
+        trayUid = p.loadURDF(os.path.join(urdfRootPath, "tray/traybox.urdf"),basePosition=[0.65,0,0])
 
         state_object= [random.uniform(0.5,0.8),random.uniform(-0.2,0.2),0.05]
         self.objectUid = p.loadURDF(os.path.join(urdfRootPath, "random_urdfs/000/000.urdf"), basePosition=state_object)
-
         state_robot = p.getLinkState(self.pandaUid, 11)[0]
         state_fingers = (p.getJointState(self.pandaUid,9)[0], p.getJointState(self.pandaUid, 10)[0])
-
         self.observation = state_robot + state_fingers
-        
-        p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,1) # rendering's back on again
-
+        p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,1)
 
         observation = np.array(self.observation).astype(np.float32)
         info = {"None" : None}
 
         return observation, info
```

