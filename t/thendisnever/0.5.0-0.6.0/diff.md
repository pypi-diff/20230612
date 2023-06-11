# Comparing `tmp/thendisnever-0.5.0.tar.gz` & `tmp/thendisnever-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thendisnever-0.5.0.tar", max compression
+gzip compressed data, was "thendisnever-0.6.0.tar", max compression
```

## Comparing `thendisnever-0.5.0.tar` & `thendisnever-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.5.0/LICENSE
--rw-r--r--   0        0        0     2682 2023-06-11 23:17:59.864149 thendisnever-0.5.0/README.md
--rw-r--r--   0        0        0      569 2023-06-11 23:18:21.824048 thendisnever-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.5.0/src/thendisnever/__init__.py
--rw-r--r--   0        0        0     4594 2023-06-11 23:20:03.343583 thendisnever-0.5.0/src/thendisnever/thend.py
--rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 thendisnever-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2682 2023-06-11 23:17:59.864149 thendisnever-0.6.0/README.md
+-rw-r--r--   0        0        0      569 2023-06-11 23:35:03.817228 thendisnever-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.6.0/src/thendisnever/__init__.py
+-rw-r--r--   0        0        0     4616 2023-06-11 23:34:56.345289 thendisnever-0.6.0/src/thendisnever/thend.py
+-rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 thendisnever-0.6.0/PKG-INFO
```

### Comparing `thendisnever-0.5.0/LICENSE` & `thendisnever-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thendisnever-0.5.0/README.md` & `thendisnever-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `thendisnever-0.5.0/pyproject.toml` & `thendisnever-0.6.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thendisnever"
-version = "0.5.0"
+version = "0.6.0"
 description = "A package to easily make an LLM talk with itself for eternity."
 authors = ["Andrew Hinh <ajhinh@gmail.com>"]
 repository = "https://github.com/andrewhinh/thendisnever"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `thendisnever-0.5.0/src/thendisnever/thend.py` & `thendisnever-0.6.0/src/thendisnever/thend.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,49 +59,52 @@
 
     # Define model.generate() arguments
     max_length = model.config.max_length  # Context window size of the model (in tokens)
     max_memory = (
         int(max_length * max_memory_ratio) + 1
     )  # Add 1 to avoid empty prompt
 
+    # Check if prompt is too long
+    inputs = tokenizer(
+        [
+            prompt
+        ],  # Wrap prompt as a list since inputs are usually a batch
+        return_tensors="pt",  # Return PyTorch tensors
+    )['input_ids'][0] # Text to tokens, index 0 because only one prompt
+    if len(inputs) >= max_length: # If the prompt is too long
+        inputs = inputs[:max_length - 1] # Only keep the first max_length - 1 tokens (- 1 to give model space to generate)
+        prompt = tokenizer.decode(
+            inputs,
+            skip_special_tokens=True,  # To remove special tokens like <eos>
+        )  # Tokens to text
+    print(prompt)  # Print the initial prompt since it's not streamed
+    
     # Set up the conversation loop, where the response is used as the next prompt
     while True:
         inputs = tokenizer(
             [
                 prompt
             ],  # Wrap prompt as a list since inputs are usually a batch
-            return_tensors="pt",  # Return PyTorch tensors
-        ) # Text to tokens
-        if len(inputs[0]) > max_length: # If the prompt is too long
-            inputs[0] = inputs[0][:max_length] # Only keep the first max_length tokens
-            prompt = tokenizer.decode(
-                inputs[0],  # index 0 since inputs are usually a batch
-                skip_special_tokens=True,  # To remove special tokens like <eos>
-            )  # Tokens to text
-            inputs = tokenizer(
-                [
-                    prompt
-                ],  # Wrap prompt as a list since inputs are usually a batch
-                return_tensors="pt",  # Return PyTorch tensors
-            )
-        print(prompt)  # Print the initial prompt since it's not streamed
+            return_tensors="pt",
+        )
         response = model.generate(
             **inputs,  # Unpack dictionary into keyword arguments
             streamer=streamer,
             max_length=max_length,
             num_return_sequences=1,  # To return only one response
             pad_token_id=tokenizer.eos_token_id,  # To remove warning message in console
             **kwargs,  # Unpack dictionary into keyword arguments
         )
         prompt = tokenizer.decode(
             response[0][
                 -max_memory:
-            ],
+            ], # index 0 since inputs are usually a batch
             skip_special_tokens=True,
         )
 
 
 # Run the function for testing
+# Arguments from here: https://huggingface.co/docs/transformers/generation_strategies#multinomial-sampling
 # isnever(
-#    do_sample=True,
-#    num_beams=1,
-# ) # Arguments from here: https://huggingface.co/docs/transformers/generation_strategies#multinomial-sampling
+#     do_sample=True,
+#     num_beams=1,
+# )
```

### Comparing `thendisnever-0.5.0/PKG-INFO` & `thendisnever-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thendisnever
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package to easily make an LLM talk with itself for eternity.
 Home-page: https://github.com/andrewhinh/thendisnever
 License: MIT
 Author: Andrew Hinh
 Author-email: ajhinh@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

