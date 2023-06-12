# Comparing `tmp/idoctorai-0.3.2.tar.gz` & `tmp/idoctorai-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.3.2.tar", max compression
+gzip compressed data, was "idoctorai-0.3.3.tar", max compression
```

## Comparing `idoctorai-0.3.2.tar` & `idoctorai-0.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.3.2/LICENSE
--rw-r--r--   0        0        0    19100 2023-06-10 07:53:33.608323 idoctorai-0.3.2/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.3.2/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.3.2/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.3.2/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.3.2/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.3.2/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.3.2/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.3.2/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.3.2/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.3.2/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2881 2023-06-10 09:03:03.357210 idoctorai-0.3.2/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.3.2/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.3.2/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11323 2023-06-10 09:13:47.773963 idoctorai-0.3.2/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.3.2/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.3.2/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.3.2/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3240 2023-06-10 07:56:37.939765 idoctorai-0.3.2/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.3.2/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.3.2/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.3.2/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.3.2/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.3.2/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.3.2/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.3.2/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1511 2023-06-08 05:58:42.812889 idoctorai-0.3.2/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1454 2023-06-10 09:14:05.013893 idoctorai-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.3.2/README.md
--rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 idoctorai-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.3.3/LICENSE
+-rw-r--r--   0        0        0    19255 2023-06-12 10:47:39.546717 idoctorai-0.3.3/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.3.3/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.3.3/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.3.3/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.3.3/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.3.3/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.3.3/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.3.3/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.3.3/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.3.3/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2909 2023-06-12 10:52:31.217546 idoctorai-0.3.3/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.3.3/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.3.3/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.3.3/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.3.3/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.3.3/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.3.3/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3240 2023-06-10 07:56:37.939765 idoctorai-0.3.3/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.3.3/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.3.3/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.3.3/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.3.3/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.3.3/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.3.3/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.3.3/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1511 2023-06-08 05:58:42.812889 idoctorai-0.3.3/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1474 2023-06-12 10:59:18.425545 idoctorai-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.3.3/README.md
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 idoctorai-0.3.3/PKG-INFO
```

### Comparing `idoctorai-0.3.2/LICENSE` & `idoctorai-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/__init__.py` & `idoctorai-0.3.3/pandasai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     _cache: Cache = Cache()
     _enable_cache: bool = True
     _prompt_id: Optional[str] = None
     last_code_generated: Optional[str] = None
     last_run_code: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
+    _history: list = None
 
     def __init__(
         self,
         llm=None,
         conversational=False,
         verbose=False,
         enforce_privacy=False,
@@ -206,14 +207,17 @@
         """
 
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
         self._prompt_id = str(uuid.uuid4())
         self.log(f"Prompt ID: {self._prompt_id}")
 
+        
+        self._history = history or []
+
         try:
             if self._enable_cache and self._cache.get(prompt):
                 self.log("Using cached response")
                 code = self._cache.get(prompt)
             else:
                 rows_to_display = 0 if self._enforce_privacy else 5
 
@@ -496,16 +500,17 @@
                             num_rows=self._original_instructions["num_rows"],
                             num_columns=self._original_instructions["num_columns"],
                             rows_to_display=self._original_instructions[
                                 "rows_to_display"
                             ],
                         )
 
+                    print(error_correcting_instruction.text)
                     code_to_run = self._llm.generate_code(
-                        error_correcting_instruction, ""
+                        error_correcting_instruction, "", self._history
                     )
 
         captured_output = output.getvalue()
 
         # Evaluate the last line and return its value or the captured output
         lines = code.strip().split("\n")
         last_line = lines[-1].strip()
```

### Comparing `idoctorai-0.3.2/pandasai/constants.py` & `idoctorai-0.3.3/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/exceptions.py` & `idoctorai-0.3.3/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/helpers/_optional.py` & `idoctorai-0.3.3/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/helpers/anonymizer.py` & `idoctorai-0.3.3/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/helpers/cache.py` & `idoctorai-0.3.3/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/helpers/from_excel.py` & `idoctorai-0.3.3/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/helpers/notebook.py` & `idoctorai-0.3.3/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/helpers/save_chart.py` & `idoctorai-0.3.3/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/langchain/__init__.py` & `idoctorai-0.3.3/pandasai/langchain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 {history}
 Human: {human_input}
 Assistant:"""
 
     def __init__(self, api_token: Optional[str] = None, **kwargs,):
         self.api_token = api_token or None
-        self.llm = OpenAI(openai_api_key=self.api_token, temperature=0, max_tokens=512)
+        self.llm = OpenAI(model_name=self.model_name, openai_api_key=self.api_token, temperature=0, max_tokens=512)
         prompt = PromptTemplate(
             input_variables=["history","human_input"], 
             template=self.template
         )
 
         memory = ConversationBufferWindowMemory(k=self.k)
         # memory = ConversationBufferMemory(memory_key="history", memory_size=3)
```

### Comparing `idoctorai-0.3.2/pandasai/llm/azure_openai.py` & `idoctorai-0.3.3/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/llm/base.py` & `idoctorai-0.3.3/pandasai/llm/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
       
         response = openai.ChatCompletion.create(**params)
 
         return response["choices"][0]["message"]["content"]
     
     def langchain_input(self, value:str, history:list = None) -> str:
         response = self.langchain.__call__(value, history)
-        # print(response)
+        print(response)
         return response
 
 
 class HuggingFaceLLM(LLM):
     """Base class to implement a new Hugging Face LLM.
 
     LLM base class is extended to be used with HuggingFace LLM Modes APIs
```

### Comparing `idoctorai-0.3.2/pandasai/llm/fake.py` & `idoctorai-0.3.3/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/llm/google_palm.py` & `idoctorai-0.3.3/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/llm/open_assistant.py` & `idoctorai-0.3.3/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/llm/openai.py` & `idoctorai-0.3.3/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/llm/starcoder.py` & `idoctorai-0.3.3/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/prompts/base.py` & `idoctorai-0.3.3/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.3.3/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.3.3/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/prompts/generate_python_code.py` & `idoctorai-0.3.3/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/prompts/generate_response.py` & `idoctorai-0.3.3/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.3.3/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.2/pyproject.toml` & `idoctorai-0.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.3.2"
+version = "0.3.3"
 description = "this is idoctorai, Generate code with natural speech"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 pandas = "1.5.3"
+openpyxl = "3.1.2"
 astor = "^0.8.1"
 openai = "^0.27.5"
 langchain = "0.0.194"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
```

### Comparing `idoctorai-0.3.2/PKG-INFO` & `idoctorai-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.3.2
+Version: 0.3.3
 Summary: this is idoctorai, Generate code with natural speech
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Provides-Extra: google
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: langchain (==0.0.194)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
+Requires-Dist: openpyxl (==3.1.2)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ## idoctorai
 
 this is idoctorai, generate code with nlp
```

