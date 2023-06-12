# Comparing `tmp/ai-coach-xblock-1.0.1.tar.gz` & `tmp/ai-coach-xblock-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-coach-xblock-1.0.1.tar", last modified: Fri Jun  9 14:39:01 2023, max compression
+gzip compressed data, was "ai-coach-xblock-1.0.2.tar", last modified: Mon Jun 12 13:47:17 2023, max compression
```

## Comparing `ai-coach-xblock-1.0.1.tar` & `ai-coach-xblock-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5778 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/ai_coach.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/static/
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/static/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/static/css/ai_coach.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/static/html/
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/static/html/ai_coach.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.007066 ai-coach-xblock-1.0.1/ai_coach/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/static/js/src/ai_coach.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-09 14:38:59.000000 ai-coach-xblock-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.791727 ai-coach-xblock-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-12 13:47:17.791727 ai-coach-xblock-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5909 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/ai_coach.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/static/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/static/css/ai_coach.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/static/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/static/html/ai_coach.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.783727 ai-coach-xblock-1.0.2/ai_coach/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/static/js/src/ai_coach.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.791727 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-12 13:47:17.791727 ai-coach-xblock-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/setup.py
```

### Comparing `ai-coach-xblock-1.0.1/LICENSE` & `ai-coach-xblock-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.1/PKG-INFO` & `ai-coach-xblock-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-coach-xblock
-Version: 1.0.1
+Version: 1.0.2
 Summary: AI Coach Xblock evaluates open response answer of a question using Open AI
 Home-page: https://github.com/edly-io/ai-feedback-xblock
 Author: edly
 License: AGPL v3
 Description: # **AI Coach XBlock**
         
         AI Coach Xblock helps learner in improving their answers by levering power of AI. It evaluates open response answer of a question using Open AI and provides feedback to learner.
```

### Comparing `ai-coach-xblock-1.0.1/README.md` & `ai-coach-xblock-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.1/ai_coach/ai_coach.py` & `ai-coach-xblock-1.0.2/ai_coach/ai_coach.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,32 +25,34 @@
             scope=Scope.settings
     )
 
     question = String(
             display_name='Question',
             default='',
             scope=Scope.settings,
-            help='The question asked by the teacher'
+            multiline_editor=True,
+            help='The question asked by the teacher',
     )
     student_answer = String(
             display_name='Answer',
             default='',
             scope=Scope.user_state,
             help='The answer provided by Student'
     )
 
     context = String(
             display_name='Context',
             default="",
             scope=Scope.settings,
+            multiline_editor=True,
             help="Write the question context here",
-            multiline=True
     )
 
     feedback_threshold = Integer(
+            display_name='Feedback Threshold',
             default=1, scope=Scope.settings,
             help="Maximum no. of times student asks for feedback"
     )
     feedback_count = Integer(
             default=0, scope=Scope.user_state,
             help="No. of times student asks for feedback"
     )
@@ -67,14 +69,15 @@
                 'text-davinci-003', 'text-davinci-002', 'text-curie-001', 'text-babbage-001',
                 'text-ada-001'),
             default="text-davinci-003", scope=Scope.settings,
             help="Select an AI Text model."
     )
 
     description = String(
+            display_name='Description',
             default='Description here...',
             scope=Scope.settings,
             help='Any Description'
     )
 
     editable_fields = [
         'display_name',
```

### Comparing `ai-coach-xblock-1.0.1/ai_coach/static/README.txt` & `ai-coach-xblock-1.0.2/ai_coach/static/README.txt`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.1/ai_coach/static/css/ai_coach.css` & `ai-coach-xblock-1.0.2/ai_coach/static/css/ai_coach.css`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 }
 
 #student-answer{
     font-size: 16px;
     font-family: var(--font-family);
     margin-bottom: 10px;
     width: 100%;
+    min-height: 150px;
 }
 
 .ai_coach_block .question-side button{
     font-size: 14px;
     padding: 4px 10px;
 }
```

### Comparing `ai-coach-xblock-1.0.1/ai_coach/static/html/ai_coach.html` & `ai-coach-xblock-1.0.2/ai_coach/static/html/ai_coach.html`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.1/ai_coach/static/js/src/ai_coach.js` & `ai-coach-xblock-1.0.2/ai_coach/static/js/src/ai_coach.js`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/PKG-INFO` & `ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-coach-xblock
-Version: 1.0.1
+Version: 1.0.2
 Summary: AI Coach Xblock evaluates open response answer of a question using Open AI
 Home-page: https://github.com/edly-io/ai-feedback-xblock
 Author: edly
 License: AGPL v3
 Description: # **AI Coach XBlock**
         
         AI Coach Xblock helps learner in improving their answers by levering power of AI. It evaluates open response answer of a question using Open AI and provides feedback to learner.
```

### Comparing `ai-coach-xblock-1.0.1/setup.py` & `ai-coach-xblock-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 data.append(os.path.relpath(os.path.join(dirname, fname), pkg))
 
     return {pkg: data}
 
 
 setup(
     name='ai-coach-xblock',
-    version='1.0.1',
+    version='1.0.2',
     description="AI Coach Xblock evaluates open response answer of a question using Open AI",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/edly-io/ai-feedback-xblock',
     license='AGPL v3',
     author='edly',
     packages=[
```

