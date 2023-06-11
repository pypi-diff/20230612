# Comparing `tmp/thendisnever-0.4.0.tar.gz` & `tmp/thendisnever-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thendisnever-0.4.0.tar", max compression
+gzip compressed data, was "thendisnever-0.5.0.tar", max compression
```

## Comparing `thendisnever-0.4.0.tar` & `thendisnever-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.4.0/LICENSE
--rw-r--r--   0        0        0     1703 2023-06-09 15:50:06.292350 thendisnever-0.4.0/README.md
--rw-r--r--   0        0        0      569 2023-06-09 15:50:14.984298 thendisnever-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.4.0/src/thendisnever/__init__.py
--rw-r--r--   0        0        0     4422 2023-06-09 16:00:27.901033 thendisnever-0.4.0/src/thendisnever/thend.py
--rw-r--r--   0        0        0     2542 1970-01-01 00:00:00.000000 thendisnever-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-07 22:53:32.798481 thendisnever-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2682 2023-06-11 23:17:59.864149 thendisnever-0.5.0/README.md
+-rw-r--r--   0        0        0      569 2023-06-11 23:18:21.824048 thendisnever-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 14:26:06.103768 thendisnever-0.5.0/src/thendisnever/__init__.py
+-rw-r--r--   0        0        0     4594 2023-06-11 23:20:03.343583 thendisnever-0.5.0/src/thendisnever/thend.py
+-rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 thendisnever-0.5.0/PKG-INFO
```

### Comparing `thendisnever-0.4.0/LICENSE` & `thendisnever-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thendisnever-0.4.0/README.md` & `thendisnever-0.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 # The End is Never
 
 A package to make an LLM talk with itself for eternity.
 
 ```python
 from thendisnever.thend import isnever
-isnever(
-  model_name='Fredithefish/ScarletPajama-3B-HF', # Default LLM
-  prompt='THE END IS NEVER THE END IS NEVER ', # Default prompt
-  max_memory_ratio=0.5 # Default % of latest tokens to remember, 0 < % < 1
-)
+isnever()
 ```
 
+## `is_never()` parameters
+
+- `model_name`: The model to generate text with.
+  - [This](https://huggingface.co/Fredithefish/ScarletPajama-3B-HF) is the default model.
+  - This must be a model compatible with `AutoModelForCausalLM` (see [here](https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoModelForCausalLM) for a list of compatible models).
+- `prompt`: The initial prompt for the model.
+  - [This](https://thestanleyparable.fandom.com/wiki/The_End_Is_Never...) is the inspiration for the default prompt.
+  - The length in tokens of the prompt must be less than the model's `max_length` (see [here](https://huggingface.co/docs/transformers/pad_truncation#padding-and-truncation) for more info).
+- `max_memory_ratio`: The % of past tokens to remember.
+  - This must be a real number between 0 and 1, since empty prompts are not allowed (0) and the prompt must be smaller than the model's context window for generation to work (1).
+- `**kwargs`: Parameters for the `model.generate()` function.
+  - See [here](https://huggingface.co/docs/transformers/generation_strategies#text-generation-strategies) for information on what parameters are available.
+
 ## Notes
 
 - When running `isnever()` for the first time, it will download the model and tokenizer from HuggingFace. This will take a while, but it only needs to be done once.
 - If you want to use the CPU (not recommended because it's slow, but it works), make sure you have [PyTorch for CPU](https://pytorch.org/get-started/locally/) installed.
 
 ## Contributing
 
@@ -39,14 +48,14 @@
 1. Test the package in a fresh environment:
 
     ```bash
     pip install dist/thendisnever-<version>.tar.gz
     ```
 
 1. Once confirmed to work, make a PR from a feature branch to main on GitHub.
-1. Once PR is merged, [email me](ajhinh@gmail.com) to be added as a collaborator on PyPI.
+1. Once PR is merged, [email me](mailto:ajhinh@gmail.com) to be added as a collaborator on PyPI.
 1. Once added as a collaborator, publish the package to `PyPI`:
   
       ```bash
       poetry config pypi-token.pypi <your-token> # Get your token from https://pypi.org/manage/account/token/
       poetry publish
       ```
```

### Comparing `thendisnever-0.4.0/pyproject.toml` & `thendisnever-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thendisnever"
-version = "0.4.0"
+version = "0.5.0"
 description = "A package to easily make an LLM talk with itself for eternity."
 authors = ["Andrew Hinh <ajhinh@gmail.com>"]
 repository = "https://github.com/andrewhinh/thendisnever"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `thendisnever-0.4.0/src/thendisnever/thend.py` & `thendisnever-0.5.0/src/thendisnever/thend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,107 @@
+# Import the necessary classes
+from transformers import (
+    AutoTokenizer, # Converts text to tokens and vice versa for the model to understand
+    AutoModelForCausalLM, # Model that generates text from a prompt
+    TextStreamer, # Print what the model generates as it generates it
+)
+
+# Define the default arguments
+DEFAULT_MODEL_NAME = "Fredithefish/ScarletPajama-3B-HF" # https://huggingface.co/Fredithefish/ScarletPajama-3B-HF
+DEFAULT_PROMPT = "THE END IS NEVER THE END IS NEVER " # https://thestanleyparable.fandom.com/wiki/The_End_Is_Never...
+DEFAULT_MAX_MEMORY_RATIO = 0.5 # Randomly chosen
+
+
+# Define the main function
 def isnever(
-    model_name="Fredithefish/ScarletPajama-3B-HF",  # LLM to use
-    prompt="THE END IS NEVER THE END IS NEVER ",  # Initial prompt to start the conversation
-    max_memory_ratio=0.5,  # % of most recent tokens in prompt to keep for the model's memory, 0 < % < 1
+    model_name=DEFAULT_MODEL_NAME, # Model to generate text with, more info here: https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoModelForCausalLM
+    prompt=DEFAULT_PROMPT, # Initial prompt for model, length (in tokens) < the model's max_length
+    max_memory_ratio=DEFAULT_MAX_MEMORY_RATIO, # % of past tokens to remember, 0 < x < 1
+    **kwargs # Parameters for the model.generate() function, more info here: https://huggingface.co/docs/transformers/generation_strategies#text-generation-strategies
 ):
-    while True:  # To retry if there's an error
-        try:  # To catch any errors
-            # To check if the parameters are valid
-            if (
-                not model_name or type(model_name) != str
-            ):  # If no model is provided or if the model is not a string
-                model_name = (
-                    "Fredithefish/ScarletPajama-3B-HF"  # To use the default model
-                )
-            if (
-                not prompt or type(prompt) != str
-            ):  # If no prompt is provided or if the prompt is not a string
-                prompt = (
-                    "THE END IS NEVER THE END IS NEVER "  # To use the default prompt
-                )
-            if (
-                not max_memory_ratio
-                or type(max_memory_ratio) != float
-                or type(max_memory_ratio) != int
-                or max_memory_ratio <= 0
-                or max_memory_ratio >= 1
-            ):
-                max_memory_ratio = 0.5  # To use the default max memory ratio
-
-            # Import the necessary classes
-            from transformers import (
-                AutoTokenizer,  # To tokenize the prompt
-                AutoModelForCausalLM,  # To generate the response
-                TextStreamer,  # To stream the response
-            )  # To import the necessary classes
-
+    # Check if the arguments are valid
+    if (
+        not model_name or type(model_name) != str
+    ):  # If no model is provided or if the model is not a string
+        model_name = DEFAULT_MODEL_NAME  # Use the default model
+    if (
+        not prompt or type(prompt) != str
+    ):
+        prompt = DEFAULT_PROMPT
+    if (
+        not max_memory_ratio
+        or type(max_memory_ratio) != float
+        or type(max_memory_ratio) != int
+        or max_memory_ratio <= 0
+        or max_memory_ratio >= 1
+    ):
+        max_memory_ratio = DEFAULT_MAX_MEMORY_RATIO
+        
+    # Download model and tokenizer, where retries are used to catch invalid model names/model download errors
+    while True:
+        try:
             # Setup the model
             model = AutoModelForCausalLM.from_pretrained(
                 model_name
-            )  # To load the model
+            )
             tokenizer = AutoTokenizer.from_pretrained(
                 model_name
-            )  # To load the tokenizer
+            )
             streamer = TextStreamer(
-                tokenizer,  # To tokenize the response
-                skip_prompt=True,  # To skip the prompt when streaming
-            )  # To create the streamer
-
-            # Setup the conversation loop
-            max_length = model.config.max_length  # To get the max length of the model
-            max_memory = (
-                int(max_length * max_memory_ratio) + 1
-            )  # To calculate the max memory of the model
-            print(prompt)  # To print the initial prompt since it's not streamed
-            while True:  # To loop the conversation
-                inputs = tokenizer(
-                    [
-                        prompt
-                    ],  # wrapping prompt as a list since inputs are usually a batch
-                    return_tensors="pt",  # To return PyTorch tensors
-                )  # To tokenize the prompt
-                response = model.generate(
-                    **inputs,  # **inputs unpacks the dictionary into keyword arguments
-                    streamer=streamer,  # To stream the response
-                    max_length=max_length,  # To limit the response length
-                    num_return_sequences=1,  # To return only one response
-                    pad_token_id=tokenizer.eos_token_id,  # To remove warning message in console
-                    # Below params inspired by this:
-                    # https://huggingface.co/docs/transformers/generation_strategies#multinomial-sampling
-                    # Check out this for more info:
-                    # https://huggingface.co/docs/transformers/generation_strategies#text-generation-strategies
-                    do_sample=True,  # To use multinomial sampling
-                    num_beams=1  # To disable beam search
-                )  # To generate the response
-                prompt = tokenizer.decode(
-                    response[0][
-                        -max_memory:
-                    ],  # index 0 since inputs are usually a batch, remove oldest tokens
-                    skip_special_tokens=True,  # To remove special tokens like <eos>
-                )  # To decode the response from tokens to text
+                tokenizer,
+                skip_prompt=True,  # To skip the prompt when streaming since it's already printed
+            )
+            break
         except OSError:  # To catch invalid model names
-            model_name = "Fredithefish/ScarletPajama-3B-HF"  # To use the default model
+            model_name = DEFAULT_MODEL_NAME  # To use the default model
             continue  # To ignore any errors and try again
         except Exception:  # To catch model download errors
             continue  # To ignore any errors and try again
 
+    # Define model.generate() arguments
+    max_length = model.config.max_length  # Context window size of the model (in tokens)
+    max_memory = (
+        int(max_length * max_memory_ratio) + 1
+    )  # Add 1 to avoid empty prompt
+
+    # Set up the conversation loop, where the response is used as the next prompt
+    while True:
+        inputs = tokenizer(
+            [
+                prompt
+            ],  # Wrap prompt as a list since inputs are usually a batch
+            return_tensors="pt",  # Return PyTorch tensors
+        ) # Text to tokens
+        if len(inputs[0]) > max_length: # If the prompt is too long
+            inputs[0] = inputs[0][:max_length] # Only keep the first max_length tokens
+            prompt = tokenizer.decode(
+                inputs[0],  # index 0 since inputs are usually a batch
+                skip_special_tokens=True,  # To remove special tokens like <eos>
+            )  # Tokens to text
+            inputs = tokenizer(
+                [
+                    prompt
+                ],  # Wrap prompt as a list since inputs are usually a batch
+                return_tensors="pt",  # Return PyTorch tensors
+            )
+        print(prompt)  # Print the initial prompt since it's not streamed
+        response = model.generate(
+            **inputs,  # Unpack dictionary into keyword arguments
+            streamer=streamer,
+            max_length=max_length,
+            num_return_sequences=1,  # To return only one response
+            pad_token_id=tokenizer.eos_token_id,  # To remove warning message in console
+            **kwargs,  # Unpack dictionary into keyword arguments
+        )
+        prompt = tokenizer.decode(
+            response[0][
+                -max_memory:
+            ],
+            skip_special_tokens=True,
+        )
+
 
-# isnever() # To test the function
+# Run the function for testing
+# isnever(
+#    do_sample=True,
+#    num_beams=1,
+# ) # Arguments from here: https://huggingface.co/docs/transformers/generation_strategies#multinomial-sampling
```

