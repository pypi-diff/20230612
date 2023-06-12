# Comparing `tmp/aitemplates-0.1.3.tar.gz` & `tmp/aitemplates-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitemplates-0.1.3.tar", max compression
+gzip compressed data, was "aitemplates-0.1.4.tar", max compression
```

## Comparing `aitemplates-0.1.3.tar` & `aitemplates-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2023-06-11 17:12:49.192362 aitemplates-0.1.3/aitemplates/__init__.py
--rw-r--r--   0        0        0     3246 2023-06-12 21:29:28.908663 aitemplates-0.1.3/aitemplates/main.py
--rw-r--r--   0        0        0        0 2023-06-11 16:53:31.418163 aitemplates-0.1.3/aitemplates/oai/__init__.py
--rw-r--r--   0        0        0      191 2023-06-11 17:06:23.567459 aitemplates-0.1.3/aitemplates/oai/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3656 2023-06-12 15:01:00.011156 aitemplates-0.1.3/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc
--rw-r--r--   0        0        0     3022 2023-06-12 21:18:51.832683 aitemplates-0.1.3/aitemplates/oai/ApiManager.py
--rw-r--r--   0        0        0        0 2023-06-11 17:03:48.721024 aitemplates-0.1.3/aitemplates/oai/responses/__init__.py
--rw-r--r--   0        0        0      201 2023-06-11 17:06:23.571195 aitemplates-0.1.3/aitemplates/oai/responses/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3128 2023-06-12 17:59:06.361492 aitemplates-0.1.3/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc
--rw-r--r--   0        0        0     1716 2023-06-12 19:04:43.677228 aitemplates-0.1.3/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc
--rw-r--r--   0        0        0     2077 2023-06-12 02:33:32.421588 aitemplates-0.1.3/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc
--rw-r--r--   0        0        0     6803 2023-06-12 21:18:51.832683 aitemplates-0.1.3/aitemplates/oai/responses/async_chat_response.py
--rw-r--r--   0        0        0     2146 2023-06-12 21:18:51.833696 aitemplates-0.1.3/aitemplates/oai/responses/chat_response.py
--rw-r--r--   0        0        0     1805 2023-06-12 21:18:51.833696 aitemplates-0.1.3/aitemplates/oai/responses/embedding.py
--rw-r--r--   0        0        0        0 2023-06-11 17:03:43.818807 aitemplates-0.1.3/aitemplates/oai/types/__init__.py
--rw-r--r--   0        0        0      197 2023-06-11 17:06:26.080642 aitemplates-0.1.3/aitemplates/oai/types/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8146 2023-06-12 15:58:45.680377 aitemplates-0.1.3/aitemplates/oai/types/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1202 2023-06-11 18:03:16.060243 aitemplates-0.1.3/aitemplates/oai/types/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0      767 2023-06-11 18:03:16.066032 aitemplates-0.1.3/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc
--rw-r--r--   0        0        0     4861 2023-06-12 21:18:52.497226 aitemplates-0.1.3/aitemplates/oai/types/base.py
--rw-r--r--   0        0        0     1703 2023-06-12 21:18:52.496213 aitemplates-0.1.3/aitemplates/oai/types/models.py
--rw-r--r--   0        0        0      403 2023-06-12 20:02:50.562326 aitemplates-0.1.3/aitemplates/oai/types/Singleton.py
--rw-r--r--   0        0        0        0 2023-06-11 17:03:56.058941 aitemplates-0.1.3/aitemplates/oai/utils/__init__.py
--rw-r--r--   0        0        0      197 2023-06-11 17:06:23.576521 aitemplates-0.1.3/aitemplates/oai/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3891 2023-06-12 15:51:23.335843 aitemplates-0.1.3/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc
--rw-r--r--   0        0        0     2381 2023-06-12 21:18:51.833696 aitemplates-0.1.3/aitemplates/oai/utils/count_tokens.py
--rw-r--r--   0        0        0     4691 2023-06-12 21:18:51.836012 aitemplates-0.1.3/aitemplates/oai/utils/wrappers.py
--rw-r--r--   0        0        0      772 2023-06-12 21:23:22.648656 aitemplates-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3049 2023-06-12 20:26:28.378694 aitemplates-0.1.3/README.md
--rw-r--r--   0        0        0     3883 1970-01-01 00:00:00.000000 aitemplates-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-11 17:12:49.192362 aitemplates-0.1.4/aitemplates/__init__.py
+-rw-r--r--   0        0        0     3308 2023-06-12 21:37:15.017128 aitemplates-0.1.4/aitemplates/main.py
+-rw-r--r--   0        0        0        0 2023-06-11 16:53:31.418163 aitemplates-0.1.4/aitemplates/oai/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-11 17:06:23.567459 aitemplates-0.1.4/aitemplates/oai/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3656 2023-06-12 15:01:00.011156 aitemplates-0.1.4/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc
+-rw-r--r--   0        0        0     3022 2023-06-12 21:18:51.832683 aitemplates-0.1.4/aitemplates/oai/ApiManager.py
+-rw-r--r--   0        0        0        0 2023-06-11 17:03:48.721024 aitemplates-0.1.4/aitemplates/oai/responses/__init__.py
+-rw-r--r--   0        0        0      201 2023-06-11 17:06:23.571195 aitemplates-0.1.4/aitemplates/oai/responses/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3128 2023-06-12 17:59:06.361492 aitemplates-0.1.4/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc
+-rw-r--r--   0        0        0     1716 2023-06-12 19:04:43.677228 aitemplates-0.1.4/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc
+-rw-r--r--   0        0        0     2077 2023-06-12 02:33:32.421588 aitemplates-0.1.4/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc
+-rw-r--r--   0        0        0     6803 2023-06-12 21:18:51.832683 aitemplates-0.1.4/aitemplates/oai/responses/async_chat_response.py
+-rw-r--r--   0        0        0     2146 2023-06-12 21:18:51.833696 aitemplates-0.1.4/aitemplates/oai/responses/chat_response.py
+-rw-r--r--   0        0        0     1805 2023-06-12 21:18:51.833696 aitemplates-0.1.4/aitemplates/oai/responses/embedding.py
+-rw-r--r--   0        0        0        0 2023-06-11 17:03:43.818807 aitemplates-0.1.4/aitemplates/oai/types/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-11 17:06:26.080642 aitemplates-0.1.4/aitemplates/oai/types/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8146 2023-06-12 15:58:45.680377 aitemplates-0.1.4/aitemplates/oai/types/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1202 2023-06-11 18:03:16.060243 aitemplates-0.1.4/aitemplates/oai/types/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0      767 2023-06-11 18:03:16.066032 aitemplates-0.1.4/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc
+-rw-r--r--   0        0        0     4861 2023-06-12 21:18:52.497226 aitemplates-0.1.4/aitemplates/oai/types/base.py
+-rw-r--r--   0        0        0     1703 2023-06-12 21:18:52.496213 aitemplates-0.1.4/aitemplates/oai/types/models.py
+-rw-r--r--   0        0        0      403 2023-06-12 20:02:50.562326 aitemplates-0.1.4/aitemplates/oai/types/Singleton.py
+-rw-r--r--   0        0        0        0 2023-06-11 17:03:56.058941 aitemplates-0.1.4/aitemplates/oai/utils/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-11 17:06:23.576521 aitemplates-0.1.4/aitemplates/oai/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3891 2023-06-12 15:51:23.335843 aitemplates-0.1.4/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc
+-rw-r--r--   0        0        0     2381 2023-06-12 21:18:51.833696 aitemplates-0.1.4/aitemplates/oai/utils/count_tokens.py
+-rw-r--r--   0        0        0     4691 2023-06-12 21:18:51.836012 aitemplates-0.1.4/aitemplates/oai/utils/wrappers.py
+-rw-r--r--   0        0        0      772 2023-06-12 21:43:20.322019 aitemplates-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3182 2023-06-12 21:42:20.041045 aitemplates-0.1.4/README.md
+-rw-r--r--   0        0        0     4016 1970-01-01 00:00:00.000000 aitemplates-0.1.4/PKG-INFO
```

### Comparing `aitemplates-0.1.3/aitemplates/main.py` & `aitemplates-0.1.4/aitemplates/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 {"chat_sequence2 = ChatSequence([description_msg, user_query_msg])" if asnc else ""}"""
 
     cell2 = nbf.v4.new_code_cell(cell2_content)
 
     db3_content = f"""
 collection.add(
     documents={"async_response1" if asnc else "[response1]"},
-    metadatas=[{{"": ""}}],
-    ids=[""]
+    metadatas=[{"{"": ""}, {"": ""}" if asnc else "{"": ""}"}],
+    ids=[{"'', ''" if asnc else "''"}]
 )"""
 
     cell3_content = f"""\
 response_list = []
 {"async_response1 = await async_create_chat_completion(ChatMessages([chat_sequence, chat_sequence2]), print_every=True, response_list=response_list)" if asnc else "response1 = create_chat_completion(chat_sequence)"}
 {db3_content if db else ""}
 {"async_response1" if asnc else "response1"}"""
```

### Comparing `aitemplates-0.1.3/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc` & `aitemplates-0.1.4/aitemplates/oai/__pycache__/ApiManager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/ApiManager.py` & `aitemplates-0.1.4/aitemplates/oai/ApiManager.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc` & `aitemplates-0.1.4/aitemplates/oai/responses/__pycache__/async_chat_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc` & `aitemplates-0.1.4/aitemplates/oai/responses/__pycache__/chat_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc` & `aitemplates-0.1.4/aitemplates/oai/responses/__pycache__/embedding.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/responses/async_chat_response.py` & `aitemplates-0.1.4/aitemplates/oai/responses/async_chat_response.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/responses/chat_response.py` & `aitemplates-0.1.4/aitemplates/oai/responses/chat_response.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/responses/embedding.py` & `aitemplates-0.1.4/aitemplates/oai/responses/embedding.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/types/__pycache__/base.cpython-39.pyc` & `aitemplates-0.1.4/aitemplates/oai/types/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/types/__pycache__/models.cpython-39.pyc` & `aitemplates-0.1.4/aitemplates/oai/types/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc` & `aitemplates-0.1.4/aitemplates/oai/types/__pycache__/Singleton.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/types/base.py` & `aitemplates-0.1.4/aitemplates/oai/types/base.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/types/models.py` & `aitemplates-0.1.4/aitemplates/oai/types/models.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc` & `aitemplates-0.1.4/aitemplates/oai/utils/__pycache__/wrappers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/utils/count_tokens.py` & `aitemplates-0.1.4/aitemplates/oai/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/aitemplates/oai/utils/wrappers.py` & `aitemplates-0.1.4/aitemplates/oai/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `aitemplates-0.1.3/pyproject.toml` & `aitemplates-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aitemplates"
-version = "0.1.3"
+version = "0.1.4"
 description = "Designed to streamline and simplify your AI workflows, it offers Python typing support, error checking, and a smart usage meter to manage API costs efficiently. Plus, it features built-in examples with ChromaDB and efficient tools for prompt engineering."
 authors = ["Silen Naihin <silen.naihin@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aitemplates"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `aitemplates-0.1.3/README.md` & `aitemplates-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -39,23 +39,23 @@
 
 ```bash
 aitemplates name_of_notebook -db -asnc
 ```
 
 ## Documentation
 
-The package includes example notebooks, which provide comprehensive guides and demonstrations of the functionalities provided by aitemplates. To access these notebooks, clone the repository and navigate to the `/notebooks` directory.
+The package includes example notebooks, which provide comprehensive guides and demonstrations of the functionalities provided by aitemplates. To access these notebooks, access or clone the repository at [https://github.com/SilenNaihin/ai_templates](https://github.com/SilenNaihin/ai_templates) and navigate to the `/notebooks` directory.
 
 Here are the available notebooks:
 
 - `oai_examples.ipynb`: Provides examples for the OpenAI API.
 - `chroma_examples.ipynb`: Demonstrates usage of ChromaDB.
 - `prompt_engineering_example.ipynb`: A comprehensive guide on prompt engineering, including various techniques, usage of ChromaDB and the OpenAI library together.
 
 ## Requirements
 
-- Be sure to have a `.env` file with the `OPENAI_API_KEY` defined in the root of your project. AWS env variables are for ChromaDB deployment https://docs.trychroma.com/deployment
-- This library doesn't currently support the use of top-p and text models like `text-davinci-003`. Streaming and logit_bias parameters are not supported
+- Be sure to have a `.env` file with the `OPENAI_API_KEY` defined in the root of your project or your api key defined in some way for OpenAI. AWS env variables are for ChromaDB deployment https://docs.trychroma.com/deployment
+- This library doesn't currently support text models like `text-davinci-003`. Streaming and logit_bias parameters are also not supported
 
 ## Contributing
 
-I'd welcome and appreciate contributions to aitemplates. If you'd like to contribute a feature, please submit a pull request. For bugs, please open a new issue, and I'll address it promptly.
+I welcome and appreciate contributions to aitemplates. If you'd like to contribute a feature, please submit a pull request. For bugs, please open a new issue, and I'll address it promptly.
```

### Comparing `aitemplates-0.1.3/PKG-INFO` & `aitemplates-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitemplates
-Version: 0.1.3
+Version: 0.1.4
 Summary: Designed to streamline and simplify your AI workflows, it offers Python typing support, error checking, and a smart usage meter to manage API costs efficiently. Plus, it features built-in examples with ChromaDB and efficient tools for prompt engineering.
 Author: Silen Naihin
 Author-email: silen.naihin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -58,24 +58,24 @@
 
 ```bash
 aitemplates name_of_notebook -db -asnc
 ```
 
 ## Documentation
 
-The package includes example notebooks, which provide comprehensive guides and demonstrations of the functionalities provided by aitemplates. To access these notebooks, clone the repository and navigate to the `/notebooks` directory.
+The package includes example notebooks, which provide comprehensive guides and demonstrations of the functionalities provided by aitemplates. To access these notebooks, access or clone the repository at [https://github.com/SilenNaihin/ai_templates](https://github.com/SilenNaihin/ai_templates) and navigate to the `/notebooks` directory.
 
 Here are the available notebooks:
 
 - `oai_examples.ipynb`: Provides examples for the OpenAI API.
 - `chroma_examples.ipynb`: Demonstrates usage of ChromaDB.
 - `prompt_engineering_example.ipynb`: A comprehensive guide on prompt engineering, including various techniques, usage of ChromaDB and the OpenAI library together.
 
 ## Requirements
 
-- Be sure to have a `.env` file with the `OPENAI_API_KEY` defined in the root of your project. AWS env variables are for ChromaDB deployment https://docs.trychroma.com/deployment
-- This library doesn't currently support the use of top-p and text models like `text-davinci-003`. Streaming and logit_bias parameters are not supported
+- Be sure to have a `.env` file with the `OPENAI_API_KEY` defined in the root of your project or your api key defined in some way for OpenAI. AWS env variables are for ChromaDB deployment https://docs.trychroma.com/deployment
+- This library doesn't currently support text models like `text-davinci-003`. Streaming and logit_bias parameters are also not supported
 
 ## Contributing
 
-I'd welcome and appreciate contributions to aitemplates. If you'd like to contribute a feature, please submit a pull request. For bugs, please open a new issue, and I'll address it promptly.
+I welcome and appreciate contributions to aitemplates. If you'd like to contribute a feature, please submit a pull request. For bugs, please open a new issue, and I'll address it promptly.
```

