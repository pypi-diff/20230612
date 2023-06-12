# Comparing `tmp/custom_diffusion-0.1.1.tar.gz` & `tmp/custom_diffusion-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_diffusion-0.1.1.tar", last modified: Sun Jun 11 10:56:52 2023, max compression
+gzip compressed data, was "custom_diffusion-0.1.2.tar", last modified: Sun Jun 11 11:55:37 2023, max compression
```

## Comparing `custom_diffusion-0.1.1.tar` & `custom_diffusion-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.429332 custom_diffusion-0.1.1/
--rw-rw-rw-   0        0        0    11558 2023-06-07 17:52:13.000000 custom_diffusion-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       24 2023-06-09 11:29:48.000000 custom_diffusion-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2595 2023-06-11 10:56:52.430313 custom_diffusion-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.384073 custom_diffusion-0.1.1/custom_diffusion/
--rw-rw-rw-   0        0        0       23 2023-06-11 10:56:31.000000 custom_diffusion-0.1.1/custom_diffusion/__init__.py
--rw-rw-rw-   0        0        0     1636 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/demo.py
-drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.416266 custom_diffusion-0.1.1/custom_diffusion/pipelines/
--rw-rw-rw-   0        0        0        0 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/pipelines/__init__.py
--rw-rw-rw-   0        0        0     6872 2023-06-10 12:22:15.000000 custom_diffusion-0.1.1/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
--rw-rw-rw-   0        0        0     7175 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/pipelines/controlnet_pipeline.py
--rw-rw-rw-   0        0        0     9308 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/preprocces.py
-drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.427323 custom_diffusion-0.1.1/custom_diffusion/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 11:02:04.000000 custom_diffusion-0.1.1/custom_diffusion/utils/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-06-11 10:45:10.000000 custom_diffusion-0.1.1/custom_diffusion/utils/data_utils.py
--rw-rw-rw-   0        0        0     1791 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/utils/downloads.py
--rw-rw-rw-   0        0        0     1307 2023-06-10 12:22:15.000000 custom_diffusion-0.1.1/custom_diffusion/utils/scheduler_utils.py
--rw-rw-rw-   0        0        0     3637 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/utils/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.411177 custom_diffusion-0.1.1/custom_diffusion.egg-info/
--rw-rw-rw-   0        0        0     2595 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-09 11:02:04.000000 custom_diffusion-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      123 2023-06-10 12:22:15.000000 custom_diffusion-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0      375 2023-06-11 10:56:52.436282 custom_diffusion-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2218 2023-06-09 11:29:48.000000 custom_diffusion-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:55:37.242984 custom_diffusion-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 17:52:13.000000 custom_diffusion-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-06-09 11:29:48.000000 custom_diffusion-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2618 2023-06-11 11:55:37.243981 custom_diffusion-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2023-06-11 10:55:21.000000 custom_diffusion-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 11:55:37.207088 custom_diffusion-0.1.2/custom_diffusion/
+-rw-rw-rw-   0        0        0       23 2023-06-11 11:55:21.000000 custom_diffusion-0.1.2/custom_diffusion/__init__.py
+-rw-rw-rw-   0        0        0     1636 2023-06-11 10:55:21.000000 custom_diffusion-0.1.2/custom_diffusion/demo.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:55:37.230027 custom_diffusion-0.1.2/custom_diffusion/pipelines/
+-rw-rw-rw-   0        0        0        0 2023-06-11 10:55:21.000000 custom_diffusion-0.1.2/custom_diffusion/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     6872 2023-06-10 12:22:15.000000 custom_diffusion-0.1.2/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
+-rw-rw-rw-   0        0        0     7330 2023-06-11 11:53:22.000000 custom_diffusion-0.1.2/custom_diffusion/pipelines/controlnet_pipeline.py
+-rw-rw-rw-   0        0        0     9308 2023-06-11 11:50:42.000000 custom_diffusion-0.1.2/custom_diffusion/preprocces.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:55:37.241004 custom_diffusion-0.1.2/custom_diffusion/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 11:02:04.000000 custom_diffusion-0.1.2/custom_diffusion/utils/__init__.py
+-rw-rw-rw-   0        0        0     2230 2023-06-11 11:53:22.000000 custom_diffusion-0.1.2/custom_diffusion/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1791 2023-06-11 10:55:21.000000 custom_diffusion-0.1.2/custom_diffusion/utils/downloads.py
+-rw-rw-rw-   0        0        0     1307 2023-06-10 12:22:15.000000 custom_diffusion-0.1.2/custom_diffusion/utils/scheduler_utils.py
+-rw-rw-rw-   0        0        0     3637 2023-06-11 10:55:21.000000 custom_diffusion-0.1.2/custom_diffusion/utils/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-11 11:55:37.223037 custom_diffusion-0.1.2/custom_diffusion.egg-info/
+-rw-rw-rw-   0        0        0     2618 2023-06-11 11:55:37.000000 custom_diffusion-0.1.2/custom_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-06-11 11:55:37.000000 custom_diffusion-0.1.2/custom_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 11:55:37.000000 custom_diffusion-0.1.2/custom_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2023-06-11 11:55:37.000000 custom_diffusion-0.1.2/custom_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-11 11:55:37.000000 custom_diffusion-0.1.2/custom_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-09 11:02:04.000000 custom_diffusion-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      123 2023-06-10 12:22:15.000000 custom_diffusion-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0      375 2023-06-11 11:55:37.245976 custom_diffusion-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2218 2023-06-09 11:29:48.000000 custom_diffusion-0.1.2/setup.py
```

### Comparing `custom_diffusion-0.1.1/LICENSE` & `custom_diffusion-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.1/PKG-INFO` & `custom_diffusion-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: custom_diffusion
-Version: 0.1.1
+Version: 0.1.2
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -64,7 +65,9 @@
      controlnet_conditioning_scale=1.0,
      generator_seed=0,
      preprocess_type="Canny",
      resize_type="center_crop_and_resize",
      crop_size=512,
 )
 ```
+
+
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: custom_diffusion Version: 0.1.1 Summary: Custom
+Metadata-Version: 2.1 Name: custom_diffusion Version: 0.1.2 Summary: Custom
 Diffusion: Creating Video from Frame Using Multiple Diffusion Home-page: https:
 //github.com/kadirnar/Custom-Diffusion Author: kadirnar License: Apache License
 2.0 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion
-models,controlnet,stable diffusion Classifier: Development Status :: 5 -
-Production/Stable Classifier: Operating System :: OS Independent Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Science/
-Research Classifier: Programming Language :: Python :: 3 Classifier:
+models,controlnet,stable diffusion Platform: UNKNOWN Classifier: Development
+Status :: 5 - Production/Stable Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.6 Description-
 Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
```

### Comparing `custom_diffusion-0.1.1/README.md` & `custom_diffusion-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.1/custom_diffusion/demo.py` & `custom_diffusion-0.1.2/custom_diffusion/demo.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.1/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py` & `custom_diffusion-0.1.2/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.1/custom_diffusion/pipelines/controlnet_pipeline.py` & `custom_diffusion-0.1.2/custom_diffusion/pipelines/controlnet_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         return generator
 
     def generate_image(
         self,
         stable_model_path: str = "runwayml/stable-diffusion-v1-5",
         controlnet_model_path: str = "lllyasviel/control_v11p_sd15_canny",
         scheduler_name: str = "DDIM",
-        image_path: str = "test.png",
+        images_list: List[str] = ["test.png"],
         prompt: List[str] = ["A photo of a cat."],
         negative_prompt: List[str] = ["bad"],
         height: int = 512,
         width: int = 512,
         guess_mode: bool = False,
         num_images_per_prompt: int = 1,
         num_inference_steps: int = 20,
@@ -156,34 +156,36 @@
         controlnet_conditioning_scale (int): The scale of controlnet conditioning in image generation.
         generator_seed (int): The seed for the random generator.
         preprocess_type (str): The type of preprocessing to apply.
 
         Returns:
         output: The generated image.
         """
-        read_image = self.load_and_resize_image(
-            image_path=image_path, resize_type=resize_type, height=height, width=width, crop_size=crop_size
-        )
-
-        control_image = preprocces_dicts[preprocess_type](read_image)
+        control_image_list = []
+        for image_path in images_list:
+            read_image = self.load_and_resize_image(
+                image_path=image_path, resize_type=resize_type, height=height, width=width, crop_size=crop_size
+            )
+            control_image = preprocces_dicts[preprocess_type](read_image)
+            control_image_list.append(control_image)
 
         pipe = self.load_model(
             stable_model_path=stable_model_path,
             controlnet_model_path=controlnet_model_path,
             scheduler_name=scheduler_name,
         )
 
         generator = self._setup_generator(generator_seed)
 
         output = pipe(
             prompt=prompt,
             height=height,
             width=width,
             guess_mode=guess_mode,
-            image=control_image,
+            image=control_image_list,
             negative_prompt=negative_prompt,
             num_images_per_prompt=num_images_per_prompt,
             num_inference_steps=num_inference_steps,
             guidance_scale=guidance_scale,
             controlnet_conditioning_scale=float(controlnet_conditioning_scale),
             generator=generator,
         ).images
```

### Comparing `custom_diffusion-0.1.1/custom_diffusion/preprocces.py` & `custom_diffusion-0.1.2/custom_diffusion/preprocces.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.1/custom_diffusion/utils/data_utils.py` & `custom_diffusion-0.1.2/custom_diffusion/utils/data_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     import os
 
     from PIL import Image
 
     images = []
     for filename in os.listdir(folder):
         if filename.endswith(".jpg") or filename.endswith(".png"):
-            img = Image.open(os.path.join(folder, filename))
+            img = os.path.join(folder, filename)
             if img is not None:
                 images.append(img)
     return images
 
 
 def center_crop_and_resize(image, crop_size, height, width):
     """
```

### Comparing `custom_diffusion-0.1.1/custom_diffusion/utils/downloads.py` & `custom_diffusion-0.1.2/custom_diffusion/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.1/custom_diffusion/utils/scheduler_utils.py` & `custom_diffusion-0.1.2/custom_diffusion/utils/scheduler_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.1/custom_diffusion/utils/video_utils.py` & `custom_diffusion-0.1.2/custom_diffusion/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.1/custom_diffusion.egg-info/PKG-INFO` & `custom_diffusion-0.1.2/custom_diffusion.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: custom-diffusion
-Version: 0.1.1
+Version: 0.1.2
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -64,7 +65,9 @@
      controlnet_conditioning_scale=1.0,
      generator_seed=0,
      preprocess_type="Canny",
      resize_type="center_crop_and_resize",
      crop_size=512,
 )
 ```
+
+
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: custom-diffusion Version: 0.1.1 Summary: Custom
+Metadata-Version: 2.1 Name: custom-diffusion Version: 0.1.2 Summary: Custom
 Diffusion: Creating Video from Frame Using Multiple Diffusion Home-page: https:
 //github.com/kadirnar/Custom-Diffusion Author: kadirnar License: Apache License
 2.0 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion
-models,controlnet,stable diffusion Classifier: Development Status :: 5 -
-Production/Stable Classifier: Operating System :: OS Independent Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Science/
-Research Classifier: Programming Language :: Python :: 3 Classifier:
+models,controlnet,stable diffusion Platform: UNKNOWN Classifier: Development
+Status :: 5 - Production/Stable Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.6 Description-
 Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
```

### Comparing `custom_diffusion-0.1.1/custom_diffusion.egg-info/SOURCES.txt` & `custom_diffusion-0.1.2/custom_diffusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.1/setup.py` & `custom_diffusion-0.1.2/setup.py`

 * *Files identical despite different names*

