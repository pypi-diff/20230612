# Comparing `tmp/une_ai-0.1.0.tar.gz` & `tmp/une_ai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "une_ai-0.1.0.tar", last modified: Tue May 16 03:11:20 2023, max compression
+gzip compressed data, was "une_ai-1.0.0.tar", last modified: Mon Jun 12 01:38:43 2023, max compression
```

## Comparing `une_ai-0.1.0.tar` & `une_ai-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-16 03:11:20.307182 une_ai-0.1.0/
--rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-0.1.0/LICENSE
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-05-16 03:11:20.307057 une_ai-0.1.0/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-05-16 03:10:04.000000 une_ai-0.1.0/README.md
--rw-r--r--   0 jonathan   (501) staff       (20)      468 2023-05-16 02:18:53.000000 une_ai-0.1.0/pyproject.toml
--rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-05-16 03:11:20.307220 une_ai-0.1.0/setup.cfg
--rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-0.1.0/setup.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-16 03:11:20.302955 une_ai-0.1.0/src/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-16 03:11:20.303771 une_ai-0.1.0/src/une_ai/
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-0.1.0/src/une_ai/__init__.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-16 03:11:20.305615 une_ai-0.1.0/src/une_ai/models/
--rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-05-16 02:01:43.000000 une_ai-0.1.0/src/une_ai/models/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5023 2023-05-15 06:11:56.000000 une_ai-0.1.0/src/une_ai/models/agent.py
--rw-r--r--   0 jonathan   (501) staff       (20)      281 2023-05-15 02:16:59.000000 une_ai-0.1.0/src/une_ai/models/environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1655 2023-05-05 11:59:19.000000 une_ai-0.1.0/src/une_ai/models/grid_map.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-16 03:11:20.306713 une_ai-0.1.0/src/une_ai/vacuum/
--rw-r--r--   0 jonathan   (501) staff       (20)      165 2023-05-16 02:09:01.000000 une_ai-0.1.0/src/une_ai/vacuum/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5041 2023-05-16 01:59:13.000000 une_ai-0.1.0/src/une_ai/vacuum/vacuum_agent.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5055 2023-05-16 01:59:27.000000 une_ai-0.1.0/src/une_ai/vacuum/vacuum_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5600 2023-05-16 02:04:46.000000 une_ai-0.1.0/src/une_ai/vacuum/vacuum_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-16 03:11:20.304644 une_ai-0.1.0/src/une_ai.egg-info/
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-05-16 03:11:20.000000 une_ai-0.1.0/src/une_ai.egg-info/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)      490 2023-05-16 03:11:20.000000 une_ai-0.1.0/src/une_ai.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 03:11:20.000000 une_ai-0.1.0/src/une_ai.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       13 2023-05-16 03:11:20.000000 une_ai-0.1.0/src/une_ai.egg-info/requires.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-05-16 03:11:20.000000 une_ai-0.1.0/src/une_ai.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.193028 une_ai-1.0.0/
+-rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-1.0.0/LICENSE
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-12 01:38:43.192891 une_ai-1.0.0/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-06-12 00:05:49.000000 une_ai-1.0.0/README.md
+-rw-r--r--   0 jonathan   (501) staff       (20)      468 2023-06-12 00:06:41.000000 une_ai-1.0.0/pyproject.toml
+-rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-06-12 01:38:43.193073 une_ai-1.0.0/setup.cfg
+-rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-1.0.0/setup.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.186353 une_ai-1.0.0/src/
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.187179 une_ai-1.0.0/src/une_ai/
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-1.0.0/src/une_ai/__init__.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.188600 une_ai-1.0.0/src/une_ai/assignments/
+-rw-r--r--   0 jonathan   (501) staff       (20)       81 2023-06-04 07:40:09.000000 une_ai-1.0.0/src/une_ai/assignments/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     7263 2023-06-04 07:45:17.000000 une_ai-1.0.0/src/une_ai/assignments/snake_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5982 2023-06-04 07:33:36.000000 une_ai-1.0.0/src/une_ai/assignments/snake_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.190461 une_ai-1.0.0/src/une_ai/models/
+-rw-r--r--   0 jonathan   (501) staff       (20)      171 2023-05-26 01:31:10.000000 une_ai-1.0.0/src/une_ai/models/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5409 2023-06-04 07:46:40.000000 une_ai-1.0.0/src/une_ai/models/agent.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      357 2023-06-04 03:18:52.000000 une_ai-1.0.0/src/une_ai/models/environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      971 2023-05-26 05:00:00.000000 une_ai-1.0.0/src/une_ai/models/game_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1311 2023-05-26 02:12:21.000000 une_ai-1.0.0/src/une_ai/models/graph_node.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     2198 2023-05-26 04:05:50.000000 une_ai-1.0.0/src/une_ai/models/grid_map.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.191735 une_ai-1.0.0/src/une_ai/tictactoe/
+-rw-r--r--   0 jonathan   (501) staff       (20)      152 2023-05-26 03:49:00.000000 une_ai-1.0.0/src/une_ai/tictactoe/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      990 2023-06-04 04:00:01.000000 une_ai-1.0.0/src/une_ai/tictactoe/tictactoc_player.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     4902 2023-06-04 04:00:39.000000 une_ai-1.0.0/src/une_ai/tictactoe/tictactoe_game.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     4536 2023-06-04 04:01:36.000000 une_ai-1.0.0/src/une_ai/tictactoe/tictactoe_game_environment.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.192527 une_ai-1.0.0/src/une_ai/vacuum/
+-rw-r--r--   0 jonathan   (501) staff       (20)      127 2023-06-06 11:05:08.000000 une_ai-1.0.0/src/une_ai/vacuum/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     8119 2023-06-06 11:02:22.000000 une_ai-1.0.0/src/une_ai/vacuum/vacuum_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5411 2023-06-06 03:24:31.000000 une_ai-1.0.0/src/une_ai/vacuum/vacuum_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-12 01:38:43.187963 une_ai-1.0.0/src/une_ai.egg-info/
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-12 01:38:42.000000 une_ai-1.0.0/src/une_ai.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)      806 2023-06-12 01:38:43.000000 une_ai-1.0.0/src/une_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-06-12 01:38:42.000000 une_ai-1.0.0/src/une_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)       13 2023-06-12 01:38:43.000000 une_ai-1.0.0/src/une_ai.egg-info/requires.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-06-12 01:38:43.000000 une_ai-1.0.0/src/une_ai.egg-info/top_level.txt
```

### Comparing `une_ai-0.1.0/LICENSE` & `une_ai-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `une_ai-0.1.0/PKG-INFO` & `une_ai-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une_ai
-Version: 0.1.0
+Version: 1.0.0
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,15 +74,15 @@
 ```
 
 Again, remember to answer y if conda asks you to install necessary dependencies.
 
 Now, to test that everything is good, let's access the Python console and import a class from the une_ai package. To access the Python3 console type:
 
 ```sh
-Python3
+python3
 ```
 
 Now that you are in the Python3 console, type the following Python commands:
 
 ```python
 from une_ai.models import GridMap
```

### Comparing `une_ai-0.1.0/README.md` & `une_ai-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 ```
 
 Again, remember to answer y if conda asks you to install necessary dependencies.
 
 Now, to test that everything is good, let's access the Python console and import a class from the une_ai package. To access the Python3 console type:
 
 ```sh
-Python3
+python3
 ```
 
 Now that you are in the Python3 console, type the following Python commands:
 
 ```python
 from une_ai.models import GridMap
```

### Comparing `une_ai-0.1.0/src/une_ai/models/agent.py` & `une_ai-1.0.0/src/une_ai/models/agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,40 @@
+import logging
 from abc import ABC, abstractmethod
 
 class Agent(ABC):
 
     def __init__(self, agent_name, agent_program):
         assert callable(agent_program), "The parameter 'agent_program' must be a function: f(Percepts) -> Actions"
 
         self._agent_name = agent_name
         self._sensors = {}
         self._actuators = {}
         self._actions = {}
         self._agent_program = agent_program
+
+        self.add_all_sensors()
+        self.add_all_actuators()
+        self.add_all_actions()
     
     def who_am_I(self):
         return self._agent_name
+    
+    # ABSTRACT methods
+
+    @abstractmethod
+    def add_all_sensors(self):
+        pass
+
+    @abstractmethod
+    def add_all_actuators(self):
+        pass
 
     @abstractmethod
-    def _interact_with_environment(self, environment):
+    def add_all_actions(self):
         pass
 
     # SENSORS methods
     
     def add_sensor(self, sensor_name, initial_value, validation_function):
         assert sensor_name not in self._sensors.keys(), "The sensor '{0}' already exists for this agent.".format(sensor_name)
         assert callable(validation_function), "The parameter validation_function must be callable."
@@ -33,17 +48,21 @@
     def _update_sensor_value(self, sensor_name, sensor_value):
         assert sensor_name in self._sensors.keys(), "The sensor '{0}' does not exist.".format(sensor_name)
         assert self._sensors[sensor_name]['validation-function'](sensor_value), "The value {0} is not a valid value for the sensor '{1}'".format(sensor_value, sensor_name)
 
         self._sensors[sensor_name]['value'] = sensor_value
     
     def sense(self, environment):
-        percepts = environment.get_percepts(self)
+        percepts = environment.get_percepts()
         for sensor_name, percept in percepts.items():
-            self._update_sensor_value(sensor_name, percept)
+            try:
+                self._update_sensor_value(sensor_name, percept)
+            except Exception as err:
+                # sensor does not exist or value is invalid
+                logging.warning(err)
     
     def read_sensor_value(self, sensor_name):
         assert sensor_name in self._sensors.keys(), "The sensor '{0}' is not a valid sensor's name".format(sensor_name)
         return self._sensors[sensor_name]['value']
     
     def read_sensors(self):
         sensors = {}
@@ -91,24 +110,23 @@
     def add_action(self, action_name, action_function):
         assert action_name not in self._actions.keys(), "The action '{0}' already exists for this agent.".format(action_name)
         assert callable(action_function), "The parameter action_function must be callable."
         
         self._actions[action_name] = action_function
 
     def act(self, actions, environment):
-        # updates the actuators based on the 
-        # chosen actions and given the action_function
-        for action in actions:
-            if action not in self._actions.keys():
-                raise KeyError("The action '{0}' is not a valid action for this agent.".format(action))
-            else:
-                updated_actuators = self._actions[action]()
-                for actuator_name, actuator_value in updated_actuators.items():
-                    self._update_actuator_value(actuator_name, actuator_value)
+        if actions is not None:
+            # updates the actuators based on the 
+            # chosen actions and given the action_function
+            for action in actions:
+                if action not in self._actions.keys():
+                    raise KeyError("The action '{0}' is not a valid action for this agent.".format(action))
+                else:
+                    updated_actuators = self._actions[action]()
+                    for actuator_name, actuator_value in updated_actuators.items():
+                        self._update_actuator_value(actuator_name, actuator_value)
         
-        # performs the actions on the environment with the
-        # updated actuators
-        self._interact_with_environment(environment)
+        environment.state_transition(self.read_actuators())
 
         return True
```

### Comparing `une_ai-0.1.0/src/une_ai/models/grid_map.py` & `une_ai-1.0.0/src/une_ai/models/grid_map.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 
 class GridMap:
-    def __init__(self, w, h, dtype=bool):
+    def __init__(self, w, h, default_value=False):
         self._w = w
         self._h = h
-        self._map = np.zeros((h, w), dtype=dtype)
+        self._default_value = default_value
+        self._map = np.array([[default_value]*w]*h) #np.zeros((h, w), dtype=dtype)
 
     def get_width(self):
         return self._w
     
     def get_height(self):
         return self._h
     
@@ -42,8 +43,18 @@
         xy_coords = []
         for coord in rc_coords:
             xy_coords.append((coord[1], coord[0]))
         
         return xy_coords
 
     def find_value(self, value):
-        return self.find_value_by_condition(lambda gridmap: gridmap == value)
+        return self.find_value_by_condition(lambda gridmap: gridmap == value)
+    
+    def set_map(self, new_map):
+        assert new_map.shape[0] == self._h and new_map.shape[1] == self._w, "The new map does not have the same dimensions of the original map. Original map dimensions {0}, new map dimensions {1}.".format(self._map.shape, new_map.shape)
+        self._map = new_map.copy()
+
+    def copy(self):
+        new_grid = GridMap(self._w, self._h, self._default_value)
+        new_grid.set_map(self._map)
+
+        return new_grid
```

### Comparing `une_ai-0.1.0/src/une_ai/vacuum/vacuum_game.py` & `une_ai-1.0.0/src/une_ai/assignments/snake_game.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,57 @@
-from une_ai.vacuum import VacuumEnvironment
-from une_ai.vacuum import VacuumAgent
+from une_ai.assignments import SnakeEnvironment
 
 import pygame
 import math
 import random
-import numpy as np
 
 BLACK = (0, 0, 0)
 WHITE = (255, 255, 255)
 RED = (255, 0, 0)
 GREEN = (0, 255, 0)
 BLUE = (0, 0, 255)
 YELLOW = (255, 255, 0)
 
 pygame.init()
-DISPLAY_WIDTH = 320
-DISPLAY_HEIGHT = 240
+DISPLAY_WIDTH = 640
+DISPLAY_HEIGHT = 480
 SCORE_BAR_HEIGHT = 40
+GAME_OVER_HEIGHT = 40
 TILE_SIZE = 10
 
 window = pygame.display.set_mode((DISPLAY_WIDTH, DISPLAY_HEIGHT+SCORE_BAR_HEIGHT))
-pygame.display.set_caption('Vacuum cleaner agent')
+pygame.display.set_caption('Assignment 1 - Snake')
 window_clock = pygame.time.Clock()
 
-class VacuumGame:
+class SnakeGame:
 
-    def __init__(self, agent_program, display_w=DISPLAY_WIDTH, display_h=DISPLAY_HEIGHT, tile_size=TILE_SIZE, max_time=60):
+    def __init__(self, snake_agent, display_w=DISPLAY_WIDTH, display_h=DISPLAY_HEIGHT, tile_size=TILE_SIZE, max_time=60, tick=5):
         self._tile_size = tile_size
         self._display = window
         self._display_size = (display_w, display_h)
         w_env = math.floor(display_w / self._tile_size)
         h_env = math.floor(display_h / self._tile_size)
-        self._environment = VacuumEnvironment(w_env, h_env)
-        empty_coords = self._environment.get_free_coords()
-        agent_pos = random.choice(empty_coords)
-        self._agent = VacuumAgent(agent_program, agent_pos[0], agent_pos[1])
-        self._agent_past_pos = (self._agent.get_pos_x(), self._agent.get_pos_y())
+        self._environment = SnakeEnvironment(w_env, h_env, max_time)
+        self._agent = snake_agent
+        # update sensors with initial state
+        self._agent.sense(self._environment)
+        self._tick = tick
 
         fonts = pygame.font.get_fonts()
         self._font = fonts[0] # default to a random font
         # try to look among the most common fonts
         test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica']
         for font in test_fonts:
             if font in fonts:
                 self._font = font
                 break
 
         self.main()
         
     def _play_step(self):
-        # this is necessary to update the color of the agent when
-        # a collision occurs
-        if not self._agent.did_collide():
-            self._agent_past_pos = (self._agent.get_pos_x(), self._agent.get_pos_y())
-        
         # SENSE
         self._agent.sense(self._environment)
         # THINK
         actions = self._agent.think()
         # ACT
         self._agent.act(actions, self._environment)
     
@@ -69,25 +63,27 @@
         y_coord = y*self._tile_size
 
         surface = pygame.Surface((self._tile_size,self._tile_size))
         surface.set_alpha(alpha) # alpha level
         pygame.draw.rect(surface, color, surface.get_rect())
         self._display.blit(surface, (x_coord, y_coord,self._tile_size,self._tile_size) )
     
-    def _draw_vacuum_agent(self):
-        color = GREEN
-        pos = (self._agent.get_pos_x(), self._agent.get_pos_y())
-        if self._agent.did_collide():
+    def _draw_snake(self):
+        if self._environment.is_game_over() and self._environment.get_time() > 0:
             color = YELLOW
-            pos = self._agent_past_pos
-        self._draw_tile(pos[0], pos[1], color)
-
-    def _draw_dirt(self):
-        dirt_coords = self._environment.get_dirt_coords()
-        for coord in dirt_coords:
+        else:
+            color = GREEN
+        percepts = self._environment.get_percepts()
+        snake_body = percepts['body-sensor']
+        for segment in snake_body:
+            self._draw_tile(segment[0], segment[1], color)
+
+    def _draw_food(self):
+        food_coords = self._environment.get_food_coords()
+        for coord in food_coords:
             self._draw_tile(coord[0], coord[1], RED)
     
     def _draw_walls(self):
         walls_coords = self._environment.get_walls_coords()
         for coord in walls_coords:
             self._draw_tile(coord[0], coord[1], WHITE)
         
@@ -98,37 +94,47 @@
             y_coord = 0
             pygame.draw.rect(self._display, WHITE, pygame.Rect(x_coord, y_coord, self._display_size[0] - x_coord, self._display_size[1]))
         if self._display_size[1] % self._tile_size > 0:
             x_coord = 0
             y_coord = self._environment.get_height()*(self._tile_size - 1)
             pygame.draw.rect(self._display, WHITE, pygame.Rect(x_coord, y_coord, self._display_size[0], self._display_size[1] - y_coord))
     
-    def _draw_explored(self):
-        explored = self._environment.get_explored_tiles_coords()
-        for coord in explored:
-            self._draw_tile(coord[0], coord[1], BLUE, 80)
-    
     def _draw_score_bar(self):
         surface = pygame.Surface((DISPLAY_WIDTH,SCORE_BAR_HEIGHT))
         pygame.draw.rect(surface, WHITE, surface.get_rect())
         self._display.blit(surface, (0, DISPLAY_HEIGHT,DISPLAY_WIDTH,SCORE_BAR_HEIGHT) )
         font = pygame.font.SysFont(self._font, 15)
         score_text = font.render("Score: {0}".format(self._environment.get_score()), True, BLACK)
-        battery_text = font.render("Battery level: {0}%".format(self._agent.get_battery_level()), True, BLACK)
+        if self._environment.is_game_over():
+            time = 0
+        else:
+            time = int(self._environment.get_time())
+        time_text = font.render("Time: {0}".format(time), True, BLACK)
         padding = 15
         self._display.blit(score_text, (padding, DISPLAY_HEIGHT+padding, int(DISPLAY_WIDTH/2)-padding, SCORE_BAR_HEIGHT))
-        self._display.blit(battery_text, (int(DISPLAY_WIDTH/2), DISPLAY_HEIGHT+padding, int(DISPLAY_WIDTH/2), SCORE_BAR_HEIGHT))
+        self._display.blit(time_text, (int(DISPLAY_WIDTH/2), DISPLAY_HEIGHT+padding, int(DISPLAY_WIDTH/2), SCORE_BAR_HEIGHT))
+    
+    def _draw_game_over(self):
+        surface = pygame.Surface((DISPLAY_WIDTH,DISPLAY_HEIGHT))
+        surface.set_alpha(60)
+        pygame.draw.rect(surface, WHITE, surface.get_rect())
+        y_pos = int((DISPLAY_HEIGHT-GAME_OVER_HEIGHT)/2)
+        self._display.blit(surface, (0, 0, DISPLAY_WIDTH,DISPLAY_HEIGHT) )
+        font = pygame.font.SysFont(self._font, 30)
+        game_over_text = font.render("GAME OVER", True, RED)
+        self._display.blit(game_over_text, (int((DISPLAY_WIDTH-150)/2), int((DISPLAY_HEIGHT-30)/2), 100, 30))
 
     def _draw_frame(self):
         self._reset_bg()
         self._draw_walls()
-        self._draw_explored()
-        self._draw_dirt()
-        self._draw_vacuum_agent()
+        self._draw_food()
+        self._draw_snake()
         self._draw_score_bar()
+        if self._environment.is_game_over():
+            self._draw_game_over()
 
     def main(self):
         running = True
 
         while running:
             # update frame
             self._draw_frame()
@@ -138,12 +144,15 @@
                 if event.type == pygame.QUIT:
                     pygame.quit()
                     running = False
                     quit()
             
             # updating game with one step
             # sense - think - act
-            self._play_step()
+            if not self._environment.is_game_over():
+                self._play_step()
 
             # Update the clock and display
             pygame.display.update()
-            window_clock.tick(5)
+            window_clock.tick(self._tick)
+            elapsed = window_clock.get_time() / 1000
+            self._environment.tick(elapsed)
```

### Comparing `une_ai-0.1.0/src/une_ai.egg-info/PKG-INFO` & `une_ai-1.0.0/src/une_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une-ai
-Version: 0.1.0
+Version: 1.0.0
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -74,15 +74,15 @@
 ```
 
 Again, remember to answer y if conda asks you to install necessary dependencies.
 
 Now, to test that everything is good, let's access the Python console and import a class from the une_ai package. To access the Python3 console type:
 
 ```sh
-Python3
+python3
 ```
 
 Now that you are in the Python3 console, type the following Python commands:
 
 ```python
 from une_ai.models import GridMap
```

