# Comparing `tmp/panda_utils-1.1.1.tar.gz` & `tmp/panda_utils-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.1.1.tar", last modified: Sun Jun 11 09:50:24 2023, max compression
+gzip compressed data, was "panda_utils-1.2.tar", last modified: Mon Jun 12 20:27:03 2023, max compression
```

## Comparing `panda_utils-1.1.1.tar` & `panda_utils-1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 09:50:24.022030 panda_utils-1.1.1/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1080 2022-08-12 11:48:21.000000 panda_utils-1.1.1/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    13891 2023-06-11 09:50:24.022030 panda_utils-1.1.1/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    13161 2023-06-11 09:22:09.000000 panda_utils-1.1.1/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.1.1/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 09:50:24.018697 panda_utils-1.1.1/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.1.1/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.1.1/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 09:50:24.022030 panda_utils-1.1.1/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.1.1/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2490 2023-06-11 09:08:34.000000 panda_utils-1.1.1/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      218 2023-06-11 09:05:00.000000 panda_utils-1.1.1/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.1.1/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     8000 2023-06-11 08:37:18.000000 panda_utils-1.1.1/panda_utils/assetpipeline/models.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 09:50:24.022030 panda_utils-1.1.1/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.1.1/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      518 2023-06-11 07:35:18.000000 panda_utils-1.1.1/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.1.1/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 09:50:24.022030 panda_utils-1.1.1/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.1.1/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5078 2022-12-14 19:53:15.000000 panda_utils-1.1.1/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      839 2023-06-10 14:24:24.000000 panda_utils-1.1.1/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 09:50:24.022030 panda_utils-1.1.1/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.1.1/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.1.1/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5348 2023-06-11 05:38:40.000000 panda_utils-1.1.1/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3587 2023-06-10 09:05:07.000000 panda_utils-1.1.1/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3184 2023-06-10 09:05:07.000000 panda_utils-1.1.1/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.1.1/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2482 2023-06-11 08:20:20.000000 panda_utils-1.1.1/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 09:50:24.018697 panda_utils-1.1.1/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    13891 2023-06-11 09:50:24.000000 panda_utils-1.1.1/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      878 2023-06-11 09:50:24.000000 panda_utils-1.1.1/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-06-11 09:50:24.000000 panda_utils-1.1.1/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-06-11 09:50:24.000000 panda_utils-1.1.1/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-06-11 09:50:24.000000 panda_utils-1.1.1/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-06-11 09:50:09.000000 panda_utils-1.1.1/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.1.1/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-06-11 09:50:24.022030 panda_utils-1.1.1/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1080 2022-08-12 11:48:21.000000 panda_utils-1.2/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    15364 2023-06-12 20:27:03.047219 panda_utils-1.2/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    14636 2023-06-12 20:11:36.000000 panda_utils-1.2/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.2/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.043886 panda_utils-1.2/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.2/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.2/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.2/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3596 2023-06-12 17:37:49.000000 panda_utils-1.2/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      218 2023-06-11 09:05:00.000000 panda_utils-1.2/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      322 2023-06-11 09:08:13.000000 panda_utils-1.2/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     8899 2023-06-12 20:24:34.000000 panda_utils-1.2/panda_utils/assetpipeline/models.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.2/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.2/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      431 2023-06-11 07:35:31.000000 panda_utils-1.2/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.2/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5178 2023-06-12 15:26:37.000000 panda_utils-1.2/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.2/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.047219 panda_utils-1.2/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.2/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.2/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.2/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3587 2023-06-10 09:05:07.000000 panda_utils-1.2/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3184 2023-06-10 09:05:07.000000 panda_utils-1.2/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.2/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2482 2023-06-12 19:50:06.000000 panda_utils-1.2/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-12 20:27:03.043886 panda_utils-1.2/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    15364 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      878 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-06-12 20:27:03.000000 panda_utils-1.2/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1021 2023-06-12 18:10:06.000000 panda_utils-1.2/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.2/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-06-12 20:27:03.047219 panda_utils-1.2/setup.cfg
```

### Comparing `panda_utils-1.1.1/LICENSE` & `panda_utils-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.1.1/PKG-INFO` & `panda_utils-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda_utils
-Version: 1.1.1
+Version: 1.2
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: imagery
 Provides-Extra: autopath
 Provides-Extra: runnable
 Provides-Extra: pipeline
 Provides-Extra: everything
 License-File: LICENSE
 
-# Panda3D Utils v1.1
+# Panda3D Utils v1.2
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -136,14 +136,17 @@
 Panda-Utils provides an asset pipeline script that can be used to build
 game-ready BAM models from models in other formats (FBX/Blend/etc.) Note that
 this process is not complete and is going to be extended in the future.
 This can be used manually through scripts, and also supports batch processing
 (for example, through Makefiles). Parallel execution works as well, as long
 as no two models have the same model name.
 
+*NOTE: the pipeline is currently in an unstable state. Expect the API to break
+a lot.*
+
 The pipeline can be started through:
 ```shell
 python -m panda_utils.assetpipeline path/to/input_folder {phase_X} {category} [step1] [step2] [...]
 ```
 
 Most of the time, the script expects a following directory structure:
 ```
@@ -167,22 +170,55 @@
 Since all changes are done in the intermediate folder, the contents of the
 input folder will not change after running this script, meaning the input
 folder can be committed into version control.
 
 Each step includes a step name and optionally arguments to that step, colon-separated.
 For example, `step_name:arg1:arg2` will call the step `step_name` with the arguments
 `arg1` and `arg2`. The steps are called in order from left to right.
+
+Any step accepting arguments can be called with `step_name[]` without any arguments.
+In that case, the step will take the arguments from a YAML file named `model-config.yml`
+in the asset input directory. It is parsed as follows:
+
+* First, the yaml field with the name = the step name is taken from the file.
+* If that field is not present, or the file is not present, the step has
+  no effect.
+* If the field is a dictionary, it will be applied as keyword arguments.
+* If the field is a list, the step will be applied once for each dictionary
+  inside of it in the proper order.
+
+This sounds confusing, so here's an example of such a config file:
+
+```yaml
+transform:
+  - scale: 10
+  - rotate: 0,0,180
+collide:
+  flags: keep,descend
+  method: polyset
+  group_name: optimized
+```
+
+When a `transform[]` action is encountered, two transform steps will be called
+in order, first the node will be rescaled, and then it will be rotated.
+When a `collide[]` action is encountered, it will be called once with the given
+arguments. If a different `[]` action is encountered, it will not run.
+This method is used for easy interaction with Makefiles (if the input folder 
+is set as the makefile dependency, changing this file will cause the task
+building a given asset to be rerun).
+
 The list of all currently existing steps is below.
 
 ### Preblend
 
 This step will convert OBJ or FBX models into BLEND. It requires installing
 Blender on the machine. Note that due to specifics of various modeling software,
 the model may end up scaled incorrectly at this phase. You can use the `transform`
-step to fix this. This step takes no arguments.
+step to fix this. All OBJ and FBX files will be joined into the same file.
+This step takes no arguments.
 
 `preblend`
 
 ### BlendRename
 
 This step will rename the BLEND models into their proper name. It is required
 if the input files are in BLEND format, but not required if the Blend files are
@@ -199,66 +235,55 @@
 with Blender 3.5.1, but is likely to work on other versions as well.
 
 This is currently using the GLTF pipeline (available since Blender 2.8),
 the builtin physics system (not bullet), and disables sRGB textures due to 
 specifics of Toontown use. It takes no arguments, but these things 
 might become configurable later through optional arguments.
 
-`blend2bam`
+* `blend2bam`
 
 ### Bam2Egg
 
 This step will decompile every BAM model into EGG models, which are used
 for processing through other methods. It takes no arguments.
 
-`bam2egg`
+* `bam2egg`
 
 ### Optimize
 
 This step will do the following transformations to every EGG model it finds:
 
-* Remaps texture paths so they work with the desirred directory structure.
-  This requires that the texture paths in the model are flat, i.e. they're
-  relative and point to a file in the same directory. `Blend2Bam` will
-  perform that conversion automatically, but if a different step is used
-  this has to be done separately.
 * Removes the default cube `Cube.N` and camera `Camera` groups from the file
   if they're found inside.
 * Creates a group with the same name as the model name, containing everything
   inside of the model. This is useful if the Panda3D code is using `find()`
   while loading this model.
 
 This function takes one required parameter `profile`. However, the profile
 is currently ignored. In the future, there will be multiple profiles that can
 (for example) run egg-optchar, etc.
 
-`optimize:stiffchar`
-`optimize:actorchar`
-`optimize:prop`
+* `optimize:stiffchar`
+* `optimize:actorchar`
+* `optimize:prop`
 
 ### Transform
 
-This step looks for a file named `transforms.yml` in the input directory.
-It will then apply the given transforms to every egg file it encounters.
-An example file can look like this:
+This step will apply the given transforms to every egg file it encounters.
+Each transform is a combination of scale, rotate, and translate. For example:
 
-```yaml
-- scale: 10
-- rotate: 0,0,180
-- translate: 0,-0.25,1
-```
+* `transform:10:0,0,180:0,-0.25,1`
 
 This will first increase the model scale 10 times, then rotate it 180 degrees
 around the Z axis (functionally setting its H angle to 180), and then translate
 it 1 unit upwards and 0.25 units backwards.
 
-This step takes no arguments. This loading method was chosen to automatically
-support batch processing through Makefiles.
+It is recommended to use the `[]` syntax to load the arguments for this step.
 
-`transform`
+* `transform[]`
 
 ### Collide
 
 This step will automatically add collision geometry to a model. This step
 will not automatically make decimated collision geometry, that has to be done
 separately. It can either add preset geometry types like Sphere, or Polyset
 geometry for complex shapes. Note that adding Polyset collisions is
@@ -273,36 +298,52 @@
   the given name. If not supplied (default), the collision will be added
   to a node with the name = input_folder's name (this group is automatically
   created by the optimize step).
 
 This step can appear multiple times in the pipeline if one wants to add
 multiple collision solids to different parts of the model. 
 
-`collide`
-`collide:keep,descend:tube`
-`collide:descend:polyset:optimized_geom`
+* `collide`
+* `collide:keep,descend:tube`
+* `collide:descend:polyset:optimized_geom`
+* `collide[]`
+
+### 3D-Palettize
+
+This step is used to join multiple texture files on a 3D model into one palette.
+It will palettize every EGG model in the folder.
+
+This step takes one parameter, the desired texture size. It must be a power
+of two. The default value is 1024, which means each produced palette will be
+1024x1024.
+
+*New in version 1.2.*
+
+* `3d_palettize`
+* `3d_palettize:2048`
 
 ### Egg2Bam
 
 This step is used to assemble the EGG model into the BAM model suitable
-for ingame use. It also copies the model into `built` folder. It takes no
-arguments.
+for ingame use. It also replaces the texture paths in the model, and 
+copies the model and every needed texture into the `built` folder.
+It takes no arguments.
 
-`egg2bam`
+* `egg2bam`
 
 ### Script
 
 This step can be used to run scripts that are not packaged with this project.
 The script will run in the directory including (transformed versions of) all
 assets in the input directory. It will receive the name of the model as its only
 argument. This step includes one parameter with the path to the script. Note that
-due to the specifics of implementation, it has to be the path, but the type
+due to the specifics of implementation, it has to be one file, but the type
 of the script is not limited (shell, python, etc.) as long as it's an executable.
 
-`script:scripts/magic.sh`
+* `script:scripts/magic.sh`
 
 For example, if your directory structure looks like this:
 
 ```
 inputs
   asset_name
     model.blend
```

### Comparing `panda_utils-1.1.1/README.md` & `panda_utils-1.2/panda_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,27 @@
-# Panda3D Utils v1.1
+Metadata-Version: 2.1
+Name: panda-utils
+Version: 1.2
+Summary: PandaUtils includes multiple tools for basic Panda3D automation
+Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
+Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
+Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: imagery
+Provides-Extra: autopath
+Provides-Extra: runnable
+Provides-Extra: pipeline
+Provides-Extra: everything
+License-File: LICENSE
+
+# Panda3D Utils v1.2
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -117,14 +136,17 @@
 Panda-Utils provides an asset pipeline script that can be used to build
 game-ready BAM models from models in other formats (FBX/Blend/etc.) Note that
 this process is not complete and is going to be extended in the future.
 This can be used manually through scripts, and also supports batch processing
 (for example, through Makefiles). Parallel execution works as well, as long
 as no two models have the same model name.
 
+*NOTE: the pipeline is currently in an unstable state. Expect the API to break
+a lot.*
+
 The pipeline can be started through:
 ```shell
 python -m panda_utils.assetpipeline path/to/input_folder {phase_X} {category} [step1] [step2] [...]
 ```
 
 Most of the time, the script expects a following directory structure:
 ```
@@ -148,22 +170,55 @@
 Since all changes are done in the intermediate folder, the contents of the
 input folder will not change after running this script, meaning the input
 folder can be committed into version control.
 
 Each step includes a step name and optionally arguments to that step, colon-separated.
 For example, `step_name:arg1:arg2` will call the step `step_name` with the arguments
 `arg1` and `arg2`. The steps are called in order from left to right.
+
+Any step accepting arguments can be called with `step_name[]` without any arguments.
+In that case, the step will take the arguments from a YAML file named `model-config.yml`
+in the asset input directory. It is parsed as follows:
+
+* First, the yaml field with the name = the step name is taken from the file.
+* If that field is not present, or the file is not present, the step has
+  no effect.
+* If the field is a dictionary, it will be applied as keyword arguments.
+* If the field is a list, the step will be applied once for each dictionary
+  inside of it in the proper order.
+
+This sounds confusing, so here's an example of such a config file:
+
+```yaml
+transform:
+  - scale: 10
+  - rotate: 0,0,180
+collide:
+  flags: keep,descend
+  method: polyset
+  group_name: optimized
+```
+
+When a `transform[]` action is encountered, two transform steps will be called
+in order, first the node will be rescaled, and then it will be rotated.
+When a `collide[]` action is encountered, it will be called once with the given
+arguments. If a different `[]` action is encountered, it will not run.
+This method is used for easy interaction with Makefiles (if the input folder 
+is set as the makefile dependency, changing this file will cause the task
+building a given asset to be rerun).
+
 The list of all currently existing steps is below.
 
 ### Preblend
 
 This step will convert OBJ or FBX models into BLEND. It requires installing
 Blender on the machine. Note that due to specifics of various modeling software,
 the model may end up scaled incorrectly at this phase. You can use the `transform`
-step to fix this. This step takes no arguments.
+step to fix this. All OBJ and FBX files will be joined into the same file.
+This step takes no arguments.
 
 `preblend`
 
 ### BlendRename
 
 This step will rename the BLEND models into their proper name. It is required
 if the input files are in BLEND format, but not required if the Blend files are
@@ -180,66 +235,55 @@
 with Blender 3.5.1, but is likely to work on other versions as well.
 
 This is currently using the GLTF pipeline (available since Blender 2.8),
 the builtin physics system (not bullet), and disables sRGB textures due to 
 specifics of Toontown use. It takes no arguments, but these things 
 might become configurable later through optional arguments.
 
-`blend2bam`
+* `blend2bam`
 
 ### Bam2Egg
 
 This step will decompile every BAM model into EGG models, which are used
 for processing through other methods. It takes no arguments.
 
-`bam2egg`
+* `bam2egg`
 
 ### Optimize
 
 This step will do the following transformations to every EGG model it finds:
 
-* Remaps texture paths so they work with the desirred directory structure.
-  This requires that the texture paths in the model are flat, i.e. they're
-  relative and point to a file in the same directory. `Blend2Bam` will
-  perform that conversion automatically, but if a different step is used
-  this has to be done separately.
 * Removes the default cube `Cube.N` and camera `Camera` groups from the file
   if they're found inside.
 * Creates a group with the same name as the model name, containing everything
   inside of the model. This is useful if the Panda3D code is using `find()`
   while loading this model.
 
 This function takes one required parameter `profile`. However, the profile
 is currently ignored. In the future, there will be multiple profiles that can
 (for example) run egg-optchar, etc.
 
-`optimize:stiffchar`
-`optimize:actorchar`
-`optimize:prop`
+* `optimize:stiffchar`
+* `optimize:actorchar`
+* `optimize:prop`
 
 ### Transform
 
-This step looks for a file named `transforms.yml` in the input directory.
-It will then apply the given transforms to every egg file it encounters.
-An example file can look like this:
+This step will apply the given transforms to every egg file it encounters.
+Each transform is a combination of scale, rotate, and translate. For example:
 
-```yaml
-- scale: 10
-- rotate: 0,0,180
-- translate: 0,-0.25,1
-```
+* `transform:10:0,0,180:0,-0.25,1`
 
 This will first increase the model scale 10 times, then rotate it 180 degrees
 around the Z axis (functionally setting its H angle to 180), and then translate
 it 1 unit upwards and 0.25 units backwards.
 
-This step takes no arguments. This loading method was chosen to automatically
-support batch processing through Makefiles.
+It is recommended to use the `[]` syntax to load the arguments for this step.
 
-`transform`
+* `transform[]`
 
 ### Collide
 
 This step will automatically add collision geometry to a model. This step
 will not automatically make decimated collision geometry, that has to be done
 separately. It can either add preset geometry types like Sphere, or Polyset
 geometry for complex shapes. Note that adding Polyset collisions is
@@ -254,36 +298,52 @@
   the given name. If not supplied (default), the collision will be added
   to a node with the name = input_folder's name (this group is automatically
   created by the optimize step).
 
 This step can appear multiple times in the pipeline if one wants to add
 multiple collision solids to different parts of the model. 
 
-`collide`
-`collide:keep,descend:tube`
-`collide:descend:polyset:optimized_geom`
+* `collide`
+* `collide:keep,descend:tube`
+* `collide:descend:polyset:optimized_geom`
+* `collide[]`
+
+### 3D-Palettize
+
+This step is used to join multiple texture files on a 3D model into one palette.
+It will palettize every EGG model in the folder.
+
+This step takes one parameter, the desired texture size. It must be a power
+of two. The default value is 1024, which means each produced palette will be
+1024x1024.
+
+*New in version 1.2.*
+
+* `3d_palettize`
+* `3d_palettize:2048`
 
 ### Egg2Bam
 
 This step is used to assemble the EGG model into the BAM model suitable
-for ingame use. It also copies the model into `built` folder. It takes no
-arguments.
+for ingame use. It also replaces the texture paths in the model, and 
+copies the model and every needed texture into the `built` folder.
+It takes no arguments.
 
-`egg2bam`
+* `egg2bam`
 
 ### Script
 
 This step can be used to run scripts that are not packaged with this project.
 The script will run in the directory including (transformed versions of) all
 assets in the input directory. It will receive the name of the model as its only
 argument. This step includes one parameter with the path to the script. Note that
-due to the specifics of implementation, it has to be the path, but the type
+due to the specifics of implementation, it has to be one file, but the type
 of the script is not limited (shell, python, etc.) as long as it's an executable.
 
-`script:scripts/magic.sh`
+* `script:scripts/magic.sh`
 
 For example, if your directory structure looks like this:
 
 ```
 inputs
   asset_name
     model.blend
```

### Comparing `panda_utils-1.1.1/panda_utils/__main__.py` & `panda_utils-1.2/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.1.1/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.2/panda_utils/assetpipeline/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import logging
 import os
 import shutil
 import sys
 
+import yaml
+
 from panda_utils.assetpipeline import imports
 from panda_utils.util import Context
 
 OUTPUT_PARENT = "built"
+# The pipeline will look for this file inside the input data whenever a [] callback is encountered
+YAML_CONFIG_FILENAME = "model-config.yml"
+logger = logging.getLogger("panda_utils.pipeline")
 
 
 class AssetContext:
     def __init__(self, input_folder, output_phase, output_folder):
         self.input_folder = input_folder
         self.output_phase = output_phase
         self.output_folder = output_folder
@@ -25,23 +30,42 @@
         self.output_model = os.path.abspath(os.path.dirname(self.intermediate_path))
         self.output_texture = os.path.abspath(f"{OUTPUT_PARENT}/{output_phase}/maps")
 
     @property
     def files(self):
         return os.listdir()
 
+    def run_action_through_config(self, action, name):
+        if YAML_CONFIG_FILENAME not in self.files:
+            return
+
+        with open(YAML_CONFIG_FILENAME) as f:
+            data = yaml.safe_load(f)
+
+        if name not in data:
+            return
+
+        args = data[name]
+        if isinstance(args, dict):
+            action(self, **args)
+        elif isinstance(args, list):
+            for kwargs in args:
+                action(self, **kwargs)
+        else:
+            logger.warning("%s: Invalid configured arguments: %s (expected list or dict)", self.name, type(args))
+
 
 def main():
     console = logging.StreamHandler()
     console.setLevel(logging.INFO)
     formatter = logging.Formatter("%(name)-12s: %(levelname)-8s %(message)s")
     console.setFormatter(formatter)
-    logger = logging.getLogger("")
-    logger.setLevel(logging.INFO)
-    logger.addHandler(console)
+    global_logger = logging.getLogger("")
+    global_logger.setLevel(logging.INFO)
+    global_logger.addHandler(console)
 
     _, input_folder, output_phase, output_folder, *pipeline = sys.argv
     ctx = AssetContext(input_folder, output_phase, output_folder)
 
     intermediate_folder = "intermediate/" + ctx.intermediate_path.replace("/", "__")
     os.makedirs("intermediate", exist_ok=True)
     if os.path.exists(intermediate_folder):
@@ -58,18 +82,28 @@
         {"options": {"panda3d_path_inherit": 1}, "paths": {"resources": resources_path}}
     )
 
     for method in pipeline:
         if not ctx.valid:
             logger.warning("The context for %s was aborted", ctx.name)
             return
-        method_name, *args = method.split(":")
+
+        if method.endswith("[]"):
+            method_name = method[:-2]
+            args = ()
+            use_config = True
+        else:
+            method_name, *args = method.split(":")
+            use_config = False
         action = imports.ALL_ACTIONS.get(method_name)
         if not action:
             logger.error("Action %s not found", method_name)
             # exit(1)
         else:
-            action(ctx, *args)
+            if use_config:
+                ctx.run_action_through_config(action, method_name)
+            else:
+                action(ctx, *args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `panda_utils-1.1.1/panda_utils/assetpipeline/models.py` & `panda_utils-1.2/panda_utils/assetpipeline/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,53 @@
 import logging
 import os
 import re
 import shutil
 import subprocess
 from pathlib import Path
 
-import yaml
 from panda_utils import util
 from panda_utils.eggtree import eggparse, operations
 from panda_utils.tools.convert import bam2egg, egg2bam
 from panda_utils.util import get_data_file_path
 
 preblend_regex = re.compile(r".*\.(fbx|obj)")
 image_regex = re.compile(r".*\.(jpg|png|rgb)")
 logger = logging.getLogger("panda_utils.pipeline.models")
 
 
-def get_filename_regex(new_name):
-    return re.compile(f"{new_name}(-[0-9]+)?.(jpg|png|rgb)")
-
-
-def remap_texture_paths(tree, new_name):
-    filename_regex = get_filename_regex(new_name)
-    textures = tree.findall("Texture")
-    remaps = {}
-    counter = 0
-    for texture in textures:
-        texture_name = texture.get_child(0)
-        texture_name_str = texture_name.value
-        if texture_name_str[0] in '"\'':
-            texture_name_str = texture_name_str[1:-1]
-        if not filename_regex.match(texture_name_str):
-            extension = texture_name_str.split(".")[-1]
-            if counter == 0:
-                new_texture_name = f"{new_name}.{extension}"
-            else:
-                new_texture_name = f"{new_name}-{counter}.{extension}"
-            counter += 1
-            remaps[texture_name_str] = new_texture_name
-            texture_name.value = f'"{new_texture_name}"'
-
-    return remaps
+def build_asset_mapper(assets, name):
+    output = {}
+    for counter, item in enumerate(assets):
+        extension = item.split(".")[-1]
+        new_file_name = f"{name}-{counter}.{extension}" if counter else f"{name}.{extension}"
+        output[item] = new_file_name
+    return output
+
+
+def get_all_textures(filename):
+    textures = []
+    with open(filename) as f:
+        eggtree = eggparse.egg_tokenize(f.readlines())
+    for tex in eggtree.findall("Texture"):
+        textures.append(tex.get_child(0).value)
+    return textures
 
 
 def action_preblend(ctx):
-    count = 0
-    for file in ctx.files:
-        if preblend_regex.match(file):
-            logger.info("%s: Converting to blend: %s", ctx.name, file)
+    all_inputs = [file for file in ctx.files if preblend_regex.match(file)]
+    logger.info("%s: Converting to blend: %s", ctx.name, ", ".join(all_inputs))
 
-            blend_filename = ctx.model_name
-            if count:
-                blend_filename += f"-{count}"
-            blend_filename += ".blend"
-            count += 1
-            subprocess.run(
-                ["blender", "--background", "--python", get_data_file_path("blender/import_model.py"),
-                 "--", file, Path.cwd() / blend_filename],
-                stdout=subprocess.DEVNULL,
-                cwd=ctx.cwd,
-            )
+    blend_filename = f"{ctx.model_name}.blend"
+    subprocess.run(
+        ["blender", "--background", "--python", get_data_file_path("blender/import_model.py"),
+         "--", Path.cwd() / blend_filename, *all_inputs],
+        stdout=subprocess.DEVNULL,
+        cwd=ctx.cwd,
+    )
 
 
 def action_blendrename(ctx):
     count = 0
     for file in ctx.files:
         if file.endswith(".blend"):
             blend_filename = ctx.model_name
@@ -105,73 +89,75 @@
             logger.info("%s: Converting %s from Bam to Egg", ctx.name, file)
             bam2egg(ctx.putil_ctx, file)
 
 
 def action_optimize(ctx, mechanism):
     logger.info("%s: Using optimization mechanism: %s", ctx.name, mechanism)
 
-    # The main thing we should do is patch the egg paths, thankfully panda-utils does that easily
+    all_eggs = {}
+    textures = set()
     for file in ctx.files:
         if file.endswith(".egg"):
-            logger.info("%s: Optimizing model: %s", ctx.name, file)
             with open(file) as f:
-                data = f.readlines()
-
-            eggtree = eggparse.egg_tokenize(data)
-            renames = remap_texture_paths(eggtree, ctx.model_name)
-            for fnold, fnnew in renames.items():
-                shutil.move(fnold, fnnew)
-                shutil.copy(fnnew, f"{ctx.output_texture}/{fnnew}")
-
-            # We also need to remove the default cube and the cameras if they're present in the model
-            nodeset = set()
+                all_eggs[file] = tree = eggparse.egg_tokenize(f.readlines())
+                for tex in tree.findall("Texture"):
+                    textures.add(eggparse.sanitize_string(tex.get_child(0).value))
+
+    texture_mapper = build_asset_mapper(textures, ctx.model_name)
+    for fnold, fnnew in texture_mapper.items():
+        shutil.move(fnold, fnnew)
+
+    for file, eggtree in all_eggs.items():
+        logger.info("%s: Optimizing model: %s", ctx.name, file)
+        # The first thing we should do is patch the texture paths
+        for tex in eggtree.findall("Texture"):
+            tex_node = tex.get_child(0)
+            tex_node.value = texture_mapper[eggparse.sanitize_string(tex_node.value)]
+
+        # We also need to remove the default cube and the cameras if they're present in the model
+        nodeset = set()
+        for node in eggtree.children:
+            if isinstance(node, eggparse.EggBranch) and node.node_type == "Group":
+                if node.node_name == "Camera" or node.node_name.startswith("Cube."):
+                    nodeset.add(node)
+        eggtree.remove_nodes(nodeset)
+
+        # For now we're also going to rename the top node into the model name, even though it's not
+        # strictly correct to do
+        if not any(group for group in eggtree.findall("Group") if group.node_name == ctx.model_name):
+            group_node = eggparse.EggBranch("Group", ctx.model_name, [])
+            removed_children = set()
             for node in eggtree.children:
                 if isinstance(node, eggparse.EggBranch) and node.node_type == "Group":
-                    if node.node_name == "Camera" or node.node_name.startswith("Cube."):
-                        nodeset.add(node)
-            eggtree.remove_nodes(nodeset)
-
-            # For now we're also going to rename the top node into the model name, even though it's not
-            # strictly correct to do
-            if not any(group for group in eggtree.findall("Group") if group.node_name == ctx.model_name):
-                for index, node in enumerate(eggtree.children):
-                    if isinstance(node, eggparse.EggBranch) and node.node_type == "Group":
-                        new_node = eggparse.EggBranch("Group", ctx.model_name, [node])
-                        eggtree.children[index] = new_node
-                        break
+                    group_node.children.append(node)
+                    removed_children.add(node)
 
-            operations.set_texture_prefix(eggtree, f"{ctx.output_phase}/maps")
-            with open(file, "w") as f:
-                f.write(str(eggtree))
+            eggtree.remove_nodes(removed_children)
+            eggtree.children.append(group_node)
 
+        with open(file, "w") as f:
+            f.write(str(eggtree))
 
-def action_transform(ctx):
-    if "transforms.yml" in ctx.files:
-        logger.info("%s: Loading transforms", ctx.name)
-        with open("transforms.yml") as f:
-            trdata = yaml.safe_load(f) or []
-    else:
-        return
 
+def action_transform(ctx, scale=None, rotate=None, translate=None):
     for file in ctx.files:
         if file.endswith(".egg"):
             logger.info("%s: Transforming: %s", ctx.name, file)
             options = []
-            for transform in trdata:
-                for key, value in transform.items():
-                    transform_type = {"scale": "TS", "rotate": "TR", "translate": "TT"}[key]
-                    options.append(f"-{transform_type}")
+            for value, transflag in [(scale, "-TS"), (rotate, "-TR"), (translate, "-TT")]:
+                if value:
+                    options.append(transflag)
                     options.append(str(value))
             if options:
                 translated_file_name = f"translated-{file}"
                 util.run_panda(ctx.putil_ctx, "egg-trans", *options, "-o", translated_file_name, file)
                 os.replace(translated_file_name, file)
 
 
-def action_collide(ctx, flags="keep,descend", method="Sphere", group_name=None):
+def action_collide(ctx, flags="keep,descend", method="sphere", group_name=None):
     group_name = group_name or ctx.model_name
     method = method.capitalize()
     flags = flags.replace(",", " ")
     for file in ctx.files:
         if file.endswith(".egg"):
             logger.info("%s: Adding collisions to %s: flags=%s method=%s", ctx.name, file, flags, method)
 
@@ -185,21 +171,67 @@
                 new_node = eggparse.EggLeaf("Collide", group_name, f"{method} {flags}")
                 groups[0].children.children.insert(0, new_node)
 
             with open(file, "w") as f:
                 f.write(str(eggtree))
 
 
+def action_3d_palettize(ctx, palette_size="1024"):
+    palette_size = int(palette_size)
+    if palette_size & (palette_size - 1):
+        raise ValueError("The palette size must be a power of two!")
+
+    logger.info("%s: Creating a TXA file...", ctx.name)
+    txa_text = (
+        f":palette {palette_size} {palette_size}\n"
+        ":imagetype png\n"
+        ":powertwo 1\n"
+        f":group {ctx.model_name} dir .\n"
+        f"*.png : force-rgba dual linear clamp_u clamp_v margin 5\n"
+    )
+    with open("textures.txa", "w") as txa_file:
+        txa_file.write(txa_text)
+
+    all_eggs = [file for file in ctx.files if file.endswith(".egg")]
+
+    logger.info("%s: Palettizing %s...", ctx.name, ', '.join(all_eggs))
+    util.run_panda(
+        ctx.putil_ctx,
+        "egg-palettize",
+        "-opt",
+        "-redo",
+        "-nodb",
+        "-inplace",
+        *all_eggs,
+        "-inplace",
+        "-tn",
+        f"{ctx.model_name}_palette_%p_%i",
+        timeout=60,
+    )
+
+
 def action_egg2bam(ctx):
     files = []
     for file in ctx.files:
         if file.endswith(".egg"):
             logger.info("%s: Copying %s into the dist directory", ctx.name, file)
-            shutil.copy(file, f"{ctx.output_model}/{file}")
             files.append(file)
+
+            with open(file) as f:
+                eggtree = eggparse.egg_tokenize(f.readlines())
+            operations.set_texture_prefix(eggtree, f"{ctx.output_phase}/maps")
+            for tex in eggtree.findall("Texture"):
+                filename = eggparse.sanitize_string(tex.get_child(0).value).split("/")[-1]
+                shutil.copy(filename, f"{ctx.output_texture}/{filename}")
+
+            with open(file, "w") as f:
+                f.write(str(eggtree))
+
+            shutil.copy(file, f"{ctx.output_model}/{file}")
+
     os.chdir(ctx.output_model)
     os.chdir(ctx.putil_ctx.resources_path)
     ctx.putil_ctx.working_path = ctx.putil_ctx.resources_path
     for file in files:
         if file.endswith(".egg"):
             logger.info("%s: Converting %s to bam", ctx.name, file)
             egg2bam(ctx.putil_ctx, ctx.output_model_rel + "/" + file)
```

### Comparing `panda_utils-1.1.1/panda_utils/blender/import_model.py` & `panda_utils-1.2/panda_utils/blender/import_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import bpy
 import sys
 
 argv = sys.argv
 argv = argv[argv.index("--") + 1:]  # get all arguments after "--"
 
-input_file, output_file = argv
+output_file, *input_files = argv
 
 
 def import_model():
     bpy.ops.object.select_all(action='SELECT')
     bpy.ops.object.delete(use_global=False)
-    if input_file.endswith("fbx"):
-        bpy.ops.import_scene.fbx(filepath=argv[0])
-    elif input_file.endswith("obj"):
-        bpy.ops.import_scene.obj(filepath=argv[0])
-    else:
-        return
+    for file in input_files:
+        if file.endswith("fbx"):
+            bpy.ops.import_scene.fbx(filepath=file)
+        elif file.endswith("obj"):
+            bpy.ops.import_scene.obj(filepath=file)
 
-    bpy.ops.wm.save_as_mainfile(filepath=argv[1])
+    bpy.ops.wm.save_as_mainfile(filepath=output_file)
 
 
 import_model()
```

### Comparing `panda_utils-1.1.1/panda_utils/eggtree/eggparse.py` & `panda_utils-1.2/panda_utils/eggtree/eggparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,20 @@
     def get_child(self, index):
         return self.children[index]
 
     def add_child(self, child):
         self.children += child
 
 
+def sanitize_string(val):
+    if val and val[0] in '"\'':
+        return val[1:-1]
+    return val
+
+
 single_line_leaf_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.]+ )?\{ ?(.+) ?}")
 preline_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.<>\"]+ )?\{([^\n]*)")
 
 
 def subtree_tokenize(lines: List[str]):
     last_line = lines[-1].strip()
     if len(lines) == 1:
```

### Comparing `panda_utils-1.1.1/panda_utils/tools/animconvert.py` & `panda_utils-1.2/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.1.1/panda_utils/tools/convert.py` & `panda_utils-1.2/panda_utils/tools/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 LODs = ["-1000", "-500", "-250"]
 
 logger = logging.getLogger("panda_utils.converter")
 
 
 def copy_single(source_path: pathlib.Path, target_path: pathlib.Path) -> None:
+    if not source_path.exists():
+        return
+
     if target_path.exists() and target_path.stat().st_mtime > source_path.stat().st_mtime:
         return
 
     target_path.parent.mkdir(parents=True, exist_ok=True)
     shutil.copytree(source_path, target_path, dirs_exist_ok=True)
```

### Comparing `panda_utils-1.1.1/panda_utils/tools/downscale.py` & `panda_utils-1.2/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.1.1/panda_utils/tools/palettize.py` & `panda_utils-1.2/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.1.1/panda_utils/tools/toontown.py` & `panda_utils-1.2/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.1.1/panda_utils/util.py` & `panda_utils-1.2/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.1.1/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,8 @@
-Metadata-Version: 2.1
-Name: panda-utils
-Version: 1.1.1
-Summary: PandaUtils includes multiple tools for basic Panda3D automation
-Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
-Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
-Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: imagery
-Provides-Extra: autopath
-Provides-Extra: runnable
-Provides-Extra: pipeline
-Provides-Extra: everything
-License-File: LICENSE
-
-# Panda3D Utils v1.1
+# Panda3D Utils v1.2
  
 This repository includes multiple tools for some basic Panda3D automation. Written in Python.
 
 ## Installation
 * `pip install panda_utils`
 * This package includes a number of optional dependencies:
   * `pip install panda_utils[imagery]` to enable the Downscale module
@@ -136,14 +117,17 @@
 Panda-Utils provides an asset pipeline script that can be used to build
 game-ready BAM models from models in other formats (FBX/Blend/etc.) Note that
 this process is not complete and is going to be extended in the future.
 This can be used manually through scripts, and also supports batch processing
 (for example, through Makefiles). Parallel execution works as well, as long
 as no two models have the same model name.
 
+*NOTE: the pipeline is currently in an unstable state. Expect the API to break
+a lot.*
+
 The pipeline can be started through:
 ```shell
 python -m panda_utils.assetpipeline path/to/input_folder {phase_X} {category} [step1] [step2] [...]
 ```
 
 Most of the time, the script expects a following directory structure:
 ```
@@ -167,22 +151,55 @@
 Since all changes are done in the intermediate folder, the contents of the
 input folder will not change after running this script, meaning the input
 folder can be committed into version control.
 
 Each step includes a step name and optionally arguments to that step, colon-separated.
 For example, `step_name:arg1:arg2` will call the step `step_name` with the arguments
 `arg1` and `arg2`. The steps are called in order from left to right.
+
+Any step accepting arguments can be called with `step_name[]` without any arguments.
+In that case, the step will take the arguments from a YAML file named `model-config.yml`
+in the asset input directory. It is parsed as follows:
+
+* First, the yaml field with the name = the step name is taken from the file.
+* If that field is not present, or the file is not present, the step has
+  no effect.
+* If the field is a dictionary, it will be applied as keyword arguments.
+* If the field is a list, the step will be applied once for each dictionary
+  inside of it in the proper order.
+
+This sounds confusing, so here's an example of such a config file:
+
+```yaml
+transform:
+  - scale: 10
+  - rotate: 0,0,180
+collide:
+  flags: keep,descend
+  method: polyset
+  group_name: optimized
+```
+
+When a `transform[]` action is encountered, two transform steps will be called
+in order, first the node will be rescaled, and then it will be rotated.
+When a `collide[]` action is encountered, it will be called once with the given
+arguments. If a different `[]` action is encountered, it will not run.
+This method is used for easy interaction with Makefiles (if the input folder 
+is set as the makefile dependency, changing this file will cause the task
+building a given asset to be rerun).
+
 The list of all currently existing steps is below.
 
 ### Preblend
 
 This step will convert OBJ or FBX models into BLEND. It requires installing
 Blender on the machine. Note that due to specifics of various modeling software,
 the model may end up scaled incorrectly at this phase. You can use the `transform`
-step to fix this. This step takes no arguments.
+step to fix this. All OBJ and FBX files will be joined into the same file.
+This step takes no arguments.
 
 `preblend`
 
 ### BlendRename
 
 This step will rename the BLEND models into their proper name. It is required
 if the input files are in BLEND format, but not required if the Blend files are
@@ -199,66 +216,55 @@
 with Blender 3.5.1, but is likely to work on other versions as well.
 
 This is currently using the GLTF pipeline (available since Blender 2.8),
 the builtin physics system (not bullet), and disables sRGB textures due to 
 specifics of Toontown use. It takes no arguments, but these things 
 might become configurable later through optional arguments.
 
-`blend2bam`
+* `blend2bam`
 
 ### Bam2Egg
 
 This step will decompile every BAM model into EGG models, which are used
 for processing through other methods. It takes no arguments.
 
-`bam2egg`
+* `bam2egg`
 
 ### Optimize
 
 This step will do the following transformations to every EGG model it finds:
 
-* Remaps texture paths so they work with the desirred directory structure.
-  This requires that the texture paths in the model are flat, i.e. they're
-  relative and point to a file in the same directory. `Blend2Bam` will
-  perform that conversion automatically, but if a different step is used
-  this has to be done separately.
 * Removes the default cube `Cube.N` and camera `Camera` groups from the file
   if they're found inside.
 * Creates a group with the same name as the model name, containing everything
   inside of the model. This is useful if the Panda3D code is using `find()`
   while loading this model.
 
 This function takes one required parameter `profile`. However, the profile
 is currently ignored. In the future, there will be multiple profiles that can
 (for example) run egg-optchar, etc.
 
-`optimize:stiffchar`
-`optimize:actorchar`
-`optimize:prop`
+* `optimize:stiffchar`
+* `optimize:actorchar`
+* `optimize:prop`
 
 ### Transform
 
-This step looks for a file named `transforms.yml` in the input directory.
-It will then apply the given transforms to every egg file it encounters.
-An example file can look like this:
+This step will apply the given transforms to every egg file it encounters.
+Each transform is a combination of scale, rotate, and translate. For example:
 
-```yaml
-- scale: 10
-- rotate: 0,0,180
-- translate: 0,-0.25,1
-```
+* `transform:10:0,0,180:0,-0.25,1`
 
 This will first increase the model scale 10 times, then rotate it 180 degrees
 around the Z axis (functionally setting its H angle to 180), and then translate
 it 1 unit upwards and 0.25 units backwards.
 
-This step takes no arguments. This loading method was chosen to automatically
-support batch processing through Makefiles.
+It is recommended to use the `[]` syntax to load the arguments for this step.
 
-`transform`
+* `transform[]`
 
 ### Collide
 
 This step will automatically add collision geometry to a model. This step
 will not automatically make decimated collision geometry, that has to be done
 separately. It can either add preset geometry types like Sphere, or Polyset
 geometry for complex shapes. Note that adding Polyset collisions is
@@ -273,36 +279,52 @@
   the given name. If not supplied (default), the collision will be added
   to a node with the name = input_folder's name (this group is automatically
   created by the optimize step).
 
 This step can appear multiple times in the pipeline if one wants to add
 multiple collision solids to different parts of the model. 
 
-`collide`
-`collide:keep,descend:tube`
-`collide:descend:polyset:optimized_geom`
+* `collide`
+* `collide:keep,descend:tube`
+* `collide:descend:polyset:optimized_geom`
+* `collide[]`
+
+### 3D-Palettize
+
+This step is used to join multiple texture files on a 3D model into one palette.
+It will palettize every EGG model in the folder.
+
+This step takes one parameter, the desired texture size. It must be a power
+of two. The default value is 1024, which means each produced palette will be
+1024x1024.
+
+*New in version 1.2.*
+
+* `3d_palettize`
+* `3d_palettize:2048`
 
 ### Egg2Bam
 
 This step is used to assemble the EGG model into the BAM model suitable
-for ingame use. It also copies the model into `built` folder. It takes no
-arguments.
+for ingame use. It also replaces the texture paths in the model, and 
+copies the model and every needed texture into the `built` folder.
+It takes no arguments.
 
-`egg2bam`
+* `egg2bam`
 
 ### Script
 
 This step can be used to run scripts that are not packaged with this project.
 The script will run in the directory including (transformed versions of) all
 assets in the input directory. It will receive the name of the model as its only
 argument. This step includes one parameter with the path to the script. Note that
-due to the specifics of implementation, it has to be the path, but the type
+due to the specifics of implementation, it has to be one file, but the type
 of the script is not limited (shell, python, etc.) as long as it's an executable.
 
-`script:scripts/magic.sh`
+* `script:scripts/magic.sh`
 
 For example, if your directory structure looks like this:
 
 ```
 inputs
   asset_name
     model.blend
```

### Comparing `panda_utils-1.1.1/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.2/panda_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_utils-1.1.1/pyproject.toml` & `panda_utils-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.1.1"
+version = "1.2"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

