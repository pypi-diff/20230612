# Comparing `tmp/langdash-1.3.2b0.tar.gz` & `tmp/langdash-1.3.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.3.2b0.tar", last modified: Mon Jun 12 08:09:22 2023, max compression
+gzip compressed data, was "langdash-1.3.2b1.tar", last modified: Mon Jun 12 09:16:40 2023, max compression
```

## Comparing `langdash-1.3.2b0.tar` & `langdash-1.3.2b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.282033 langdash-1.3.2b0/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.2b0/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.2b0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     2909 2023-06-12 08:09:22.282033 langdash-1.3.2b0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1970 2023-06-12 02:45:52.000000 langdash-1.3.2b0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.278033 langdash-1.3.2b0/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       77 2023-06-12 08:08:14.000000 langdash-1.3.2b0/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.282033 langdash-1.3.2b0/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14690 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     8091 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.278033 langdash-1.3.2b0/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.2b0/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1967 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-06-12 02:43:18.000000 langdash-1.3.2b0/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      777 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.2b0/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.2b0/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.282033 langdash-1.3.2b0/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.2b0/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.3.2b0/langdash/models/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     7647 2023-06-12 08:08:14.000000 langdash-1.3.2b0/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     7274 2023-06-12 08:08:14.000000 langdash-1.3.2b0/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.2b0/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)    10150 2023-06-12 08:08:14.000000 langdash-1.3.2b0/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.3.2b0/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     7534 2023-06-10 07:12:57.000000 langdash-1.3.2b0/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.2b0/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2741 2023-06-10 03:12:00.000000 langdash-1.3.2b0/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.278033 langdash-1.3.2b0/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.2b0/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1098 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.2b0/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.2b0/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.282033 langdash-1.3.2b0/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2909 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1337 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      297 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 08:09:22.282033 langdash-1.3.2b0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1704 2023-06-12 08:08:14.000000 langdash-1.3.2b0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 09:16:40.330156 langdash-1.3.2b1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.2b1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.2b1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-12 09:16:40.330156 langdash-1.3.2b1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-12 09:16:01.000000 langdash-1.3.2b1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 09:16:40.326156 langdash-1.3.2b1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-12 09:16:35.000000 langdash-1.3.2b1/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 09:16:40.330156 langdash-1.3.2b1/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.2b1/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14690 2023-06-11 03:43:22.000000 langdash-1.3.2b1/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8091 2023-06-11 03:43:22.000000 langdash-1.3.2b1/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.2b1/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 09:16:40.326156 langdash-1.3.2b1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.2b1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1967 2023-06-11 03:43:22.000000 langdash-1.3.2b1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-06-12 02:43:18.000000 langdash-1.3.2b1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      777 2023-06-11 03:43:22.000000 langdash-1.3.2b1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.2b1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.2b1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 09:16:40.330156 langdash-1.3.2b1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.2b1/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.3.2b1/langdash/models/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7647 2023-06-12 08:08:14.000000 langdash-1.3.2b1/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7274 2023-06-12 08:08:14.000000 langdash-1.3.2b1/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.2b1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10150 2023-06-12 08:08:14.000000 langdash-1.3.2b1/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.3.2b1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7534 2023-06-10 07:12:57.000000 langdash-1.3.2b1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.2b1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2741 2023-06-10 03:12:00.000000 langdash-1.3.2b1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 09:16:40.326156 langdash-1.3.2b1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.2b1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1098 2023-06-11 03:43:22.000000 langdash-1.3.2b1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.2b1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.2b1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 09:16:40.326156 langdash-1.3.2b1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-12 09:16:40.000000 langdash-1.3.2b1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1337 2023-06-12 09:16:40.000000 langdash-1.3.2b1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 09:16:40.000000 langdash-1.3.2b1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      297 2023-06-12 09:16:40.000000 langdash-1.3.2b1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-12 09:16:40.000000 langdash-1.3.2b1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 09:16:40.330156 langdash-1.3.2b1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1704 2023-06-12 08:08:14.000000 langdash-1.3.2b1/setup.py
```

### Comparing `langdash-1.3.2b0/LICENSE.txt` & `langdash-1.3.2b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/PKG-INFO` & `langdash-1.3.2b1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,14 @@
-Metadata-Version: 2.1
-Name: langdash
-Version: 1.3.2b0
-Summary: A simple library for interfacing with language models.
-Home-page: https://git.mysymphony.jp.net/nana/langdash
-Author: Nana Mochizuki
-Author-email: nana@mysymphony.jp.net
-Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
-Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: embeddings
-Provides-Extra: rwkv_cpp
-Provides-Extra: llama_cpp
-Provides-Extra: transformers
-Provides-Extra: ctransformers
-Provides-Extra: sentence_transformers
-License-File: LICENSE.txt
-
 # langdash
 
 [**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
 
 A simple library for interfacing with language models.
 
-**Currently in alpha!**
+**Currently in beta!**
 
 **Features:**
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends.
@@ -66,10 +41,31 @@
 
   * [Text generation](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/text-generation.md)
   * [Generating TV shows](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/generating-tv-shows.md)
   * [Embedding search](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/embedding-search.md)
 
 See [examples folder](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/examples) for full examples.
 
+## Running the Examples
+
+All examples can be ran with the following command:
+
+```
+python examples/instruct.py [model type] [model name or path]
+```
+
+You can specify additional model parameters using the `-ae` CLI argument, and passing a valid Python literal. For example, to run the chat example using the WizardLM model with context length of 4096, do:
+
+```
+python examples/chat.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096
+```
+
+Some examples require you to specify the prompt format. Currently, two are implemented: WizardLM (shortened Alpaca format without the first prompt line and `# Instruction:`), and Alpaca (the full format). You'll need to specify it for most of the other examples:
+
+```
+python examples/instruct.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096 --prompt-format wizardlm
+```
+
+
 ## License
 
-Apache 2.0
+Apache 2.0
```

### Comparing `langdash-1.3.2b0/langdash/chains/chains.py` & `langdash-1.3.2b1/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/chains/nodes.py` & `langdash-1.3.2b1/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/classify/token_qa.py` & `langdash-1.3.2b1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/core.py` & `langdash-1.3.2b1/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/infer.py` & `langdash-1.3.2b1/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/llm.py` & `langdash-1.3.2b1/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/llm_session.py` & `langdash-1.3.2b1/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/models/_bpe.py` & `langdash-1.3.2b1/langdash/models/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/models/ctransformers.py` & `langdash-1.3.2b1/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/models/llama_cpp.py` & `langdash-1.3.2b1/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/models/mock.py` & `langdash-1.3.2b1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/models/rwkv_cpp.py` & `langdash-1.3.2b1/langdash/models/rwkv_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/models/sentence_transformers.py` & `langdash-1.3.2b1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/models/transformers.py` & `langdash-1.3.2b1/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/response.py` & `langdash-1.3.2b1/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/sampling.py` & `langdash-1.3.2b1/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/search/embedding_search.py` & `langdash-1.3.2b1/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/search/engine.py` & `langdash-1.3.2b1/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash/search/multichoice_search.py` & `langdash-1.3.2b1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/langdash.egg-info/SOURCES.txt` & `langdash-1.3.2b1/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.2b0/setup.py` & `langdash-1.3.2b1/setup.py`

 * *Files identical despite different names*

