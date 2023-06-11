# Comparing `tmp/panml-1.0.3.tar.gz` & `tmp/panml-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-1.0.3.tar", last modified: Sun Jun 11 00:55:43 2023, max compression
+gzip compressed data, was "panml-1.0.4.tar", last modified: Sun Jun 11 23:54:53 2023, max compression
```

## Comparing `panml-1.0.3.tar` & `panml-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.800030 panml-1.0.3/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.3/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-11 00:55:43.800292 panml-1.0.3/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.3/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.791232 panml-1.0.3/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.3/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.794530 panml-1.0.3/panml/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.3/panml/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-06-08 13:09:32.000000 panml-1.0.3/panml/clustering/faiss.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.3/panml/constants.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.3/panml/environments.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.796905 panml-1.0.3/panml/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.3/panml/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    24206 2023-06-11 00:54:36.000000 panml-1.0.3/panml/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    15676 2023-06-08 13:09:32.000000 panml-1.0.3/panml/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-11 00:13:19.000000 panml-1.0.3/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.3/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.793524 panml-1.0.3/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-11 00:55:43.000000 panml-1.0.3/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-11 00:55:43.801182 panml-1.0.3/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-11 00:54:36.000000 panml-1.0.3/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 00:55:43.799103 panml-1.0.3/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.3/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-1.0.3/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.229612 panml-1.0.4/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.4/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-11 23:54:53.229876 panml-1.0.4/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.4/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.222976 panml-1.0.4/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.4/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.225399 panml-1.0.4/panml/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.4/panml/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-06-08 13:09:32.000000 panml-1.0.4/panml/clustering/faiss.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.4/panml/constants.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.4/panml/environments.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.226875 panml-1.0.4/panml/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.4/panml/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    24206 2023-06-11 00:54:36.000000 panml-1.0.4/panml/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    15604 2023-06-11 23:54:12.000000 panml-1.0.4/panml/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-11 00:13:19.000000 panml-1.0.4/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.4/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.224777 panml-1.0.4/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-11 23:54:53.230605 panml-1.0.4/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-11 23:54:12.000000 panml-1.0.4/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.228330 panml-1.0.4/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.4/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-1.0.4/test/test_VectorEngine.py
```

### Comparing `panml-1.0.3/LICENSE` & `panml-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-1.0.3/PKG-INFO` & `panml-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.3
+Version: 1.0.4
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.3/README.md` & `panml-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `panml-1.0.3/panml/clustering/faiss.py` & `panml-1.0.4/panml/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.3/panml/constants.py` & `panml-1.0.4/panml/constants.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.3/panml/environments.py` & `panml-1.0.4/panml/environments.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.3/panml/llm/huggingface.py` & `panml-1.0.4/panml/llm/huggingface.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.3/panml/llm/openai.py` & `panml-1.0.4/panml/llm/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,24 +196,24 @@
                     output_context['text'] = output_context['text'].replace('\n', ' ').replace('\xa0', '').replace('  ', ' ')
                     output_context['text'] = output_context['text'].replace(',', ', ')
                     output_context['text'] = output_context['text'].replace('.', '. ')
                     output_context['text'] = output_context['text'].replace('  ', ' ')
                     if len(output_context['text'].replace(' ', '')) < 2:
                         break
 
-                    history.append(output_context)
-            
-                    try:
-                        if keep_history:
-                            prediction.append(history[-1]) # saves last prediction output
-                            self.prediction_history.append(history) # saves all historical prediction output
-                        else:
-                            prediction.append(history[-1])
-                    except:
-                        prediction.append({'text': None}) # if there is invalid response from the language model, return None
+                history.append(output_context)
+        
+            try:
+                if keep_history:
+                    prediction.append(history[-1]) # saves last prediction output
+                    self.prediction_history.append(history) # saves all historical prediction output
+                else:
+                    prediction.append(history[-1])
+            except:
+                prediction.append({'text': None}) # if there is invalid response from the language model, return None
 
         # Gather output
         if isinstance(text, str):
             return prediction[0] # return string text as result
         else:
             if display_probability:
                 return prediction # return list of output_context dict as result
```

### Comparing `panml-1.0.3/panml/models.py` & `panml-1.0.4/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.3/panml/search.py` & `panml-1.0.4/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.3/panml.egg-info/PKG-INFO` & `panml-1.0.4/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.3
+Version: 1.0.4
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.3/setup.py` & `panml-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '1.0.3', # version
+  version = '1.0.4', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-1.0.3/test/test_ModelPack.py` & `panml-1.0.4/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.3/test/test_VectorEngine.py` & `panml-1.0.4/test/test_VectorEngine.py`

 * *Files identical despite different names*

