# Comparing `tmp/langdash-1.3.1a0.tar.gz` & `tmp/langdash-1.3.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.3.1a0.tar", last modified: Mon Jun 12 02:47:43 2023, max compression
+gzip compressed data, was "langdash-1.3.2b0.tar", last modified: Mon Jun 12 08:09:22 2023, max compression
```

## Comparing `langdash-1.3.1a0.tar` & `langdash-1.3.2b0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 02:47:43.848743 langdash-1.3.1a0/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.1a0/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.1a0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     2909 2023-06-12 02:47:43.848743 langdash-1.3.1a0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1970 2023-06-12 02:45:52.000000 langdash-1.3.1a0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 02:47:43.844743 langdash-1.3.1a0/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       77 2023-06-12 02:47:35.000000 langdash-1.3.1a0/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 02:47:43.848743 langdash-1.3.1a0/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.1a0/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14690 2023-06-11 03:43:22.000000 langdash-1.3.1a0/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     8091 2023-06-11 03:43:22.000000 langdash-1.3.1a0/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.1a0/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 02:47:43.844743 langdash-1.3.1a0/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.1a0/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1967 2023-06-11 03:43:22.000000 langdash-1.3.1a0/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-06-12 02:43:18.000000 langdash-1.3.1a0/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      777 2023-06-11 03:43:22.000000 langdash-1.3.1a0/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.1a0/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.1a0/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 02:47:43.848743 langdash-1.3.1a0/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.1a0/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.3.1a0/langdash/models/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     7663 2023-06-12 02:43:18.000000 langdash-1.3.1a0/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     7092 2023-06-10 00:53:03.000000 langdash-1.3.1a0/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.1a0/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     9918 2023-06-11 04:47:55.000000 langdash-1.3.1a0/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.3.1a0/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     7534 2023-06-10 07:12:57.000000 langdash-1.3.1a0/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.1a0/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2741 2023-06-10 03:12:00.000000 langdash-1.3.1a0/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 02:47:43.844743 langdash-1.3.1a0/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.1a0/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1098 2023-06-11 03:43:22.000000 langdash-1.3.1a0/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.1a0/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.1a0/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 02:47:43.844743 langdash-1.3.1a0/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2909 2023-06-12 02:47:43.000000 langdash-1.3.1a0/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1337 2023-06-12 02:47:43.000000 langdash-1.3.1a0/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 02:47:43.000000 langdash-1.3.1a0/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      267 2023-06-12 02:47:43.000000 langdash-1.3.1a0/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-12 02:47:43.000000 langdash-1.3.1a0/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 02:47:43.848743 langdash-1.3.1a0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1674 2023-06-12 02:43:18.000000 langdash-1.3.1a0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.282033 langdash-1.3.2b0/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.2b0/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.2b0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     2909 2023-06-12 08:09:22.282033 langdash-1.3.2b0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1970 2023-06-12 02:45:52.000000 langdash-1.3.2b0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.278033 langdash-1.3.2b0/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       77 2023-06-12 08:08:14.000000 langdash-1.3.2b0/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.282033 langdash-1.3.2b0/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14690 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8091 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.278033 langdash-1.3.2b0/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.2b0/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1967 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-06-12 02:43:18.000000 langdash-1.3.2b0/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      777 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.2b0/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.2b0/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.282033 langdash-1.3.2b0/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.2b0/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.3.2b0/langdash/models/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7647 2023-06-12 08:08:14.000000 langdash-1.3.2b0/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7274 2023-06-12 08:08:14.000000 langdash-1.3.2b0/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.2b0/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10150 2023-06-12 08:08:14.000000 langdash-1.3.2b0/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.3.2b0/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7534 2023-06-10 07:12:57.000000 langdash-1.3.2b0/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.2b0/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2741 2023-06-10 03:12:00.000000 langdash-1.3.2b0/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.278033 langdash-1.3.2b0/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.2b0/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1098 2023-06-11 03:43:22.000000 langdash-1.3.2b0/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.2b0/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.2b0/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 08:09:22.282033 langdash-1.3.2b0/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2909 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1337 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      297 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-12 08:09:22.000000 langdash-1.3.2b0/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 08:09:22.282033 langdash-1.3.2b0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1704 2023-06-12 08:08:14.000000 langdash-1.3.2b0/setup.py
```

### Comparing `langdash-1.3.1a0/LICENSE.txt` & `langdash-1.3.2b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/PKG-INFO` & `langdash-1.3.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.3.1a0
+Version: 1.3.2b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.3.1a0/README.md` & `langdash-1.3.2b0/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/chains/chains.py` & `langdash-1.3.2b0/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/chains/nodes.py` & `langdash-1.3.2b0/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/classify/token_qa.py` & `langdash-1.3.2b0/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/core.py` & `langdash-1.3.2b0/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/infer.py` & `langdash-1.3.2b0/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/llm.py` & `langdash-1.3.2b0/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/llm_session.py` & `langdash-1.3.2b0/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/models/_bpe.py` & `langdash-1.3.2b0/langdash/models/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/models/ctransformers.py` & `langdash-1.3.2b0/langdash/models/llama_cpp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,91 @@
-from typing import Generator, List, Optional, Union, Dict, Any, Set
+from typing import Generator, List, Optional, Union
 from math import inf
 import weakref
 
 import torch
+from llama_cpp import Llama, LlamaState, llama_token_to_str  #type: ignore
 
 from langdash.response import RespInfer
 from langdash.llm import LLM
 from langdash.llm_session import LLMGenerationSessionForRawText
 from langdash.infer import InferArgs
 import langdash.sampling as sampling
-import langdash.models._bpe as bpe
+from ._tokenizer.bytes_dict_tokenizer import BytesDictTokenizer, BytesDictBufferedToken
 
-import ctransformers # type: ignore
-from ctransformers.llm import LLM as CTransformersLLM, LLMState as CTransformersState # type: ignore
 
-class CTransformersWrapper:
-  model: CTransformersLLM
-  tokenizer: Optional[Any]
-  buffered_token_head: Set[int]
-  vocab: Dict[str, int]
+class LlamaWrapper:
+  model: Llama
+  tokenizer: BytesDictTokenizer
   last_called_session: Optional[weakref.ref]
+  eos_token: int
+  bos_token: int
 
-  def __init__(self, model_path: str, tokenizer: Optional[Any] = None, *args, **kwargs):
-    self.model = ctransformers.AutoModelForCausalLM.from_pretrained(model_path, **kwargs)
-    if tokenizer:
-      self.tokenizer = tokenizer
-      import transformers
-      if isinstance(
-        tokenizer, (transformers.GPT2Tokenizer, transformers.GPT2TokenizerFast)
-      ):
-        self.vocab = {
-          bpe.decode(logits_tokstr): logits_tokid
-          for logits_tokstr, logits_tokid in tokenizer.get_vocab().items()
-        }
-        self.buffered_token_head = set(
-          v for k, v in tokenizer.get_vocab().items() if "\u0122" in k
-        )
-      else:
-        self.vocab = tokenizer.get_vocab()
-        self.buffered_token_head = set()
-    else:
-      self.tokenizer = tokenizer
-      self.vocab = {}
-      self.buffered_token_head = set()
+  def __init__(self, *args, **kwargs):
+    self.model = Llama(*args, **kwargs)
+    mapping = [
+      llama_token_to_str(self.model.ctx, tokid)
+      for tokid in range(self.model.n_vocab())
+    ]
+    self.tokenizer = BytesDictTokenizer(
+      lambda text, **_k: self.model.
+      tokenize(text.encode("utf-8"), add_bos=False),
+      lambda tokens, **_k: self.model.detokenize(tokens).decode("utf-8"),
+      mapping
+    )
     self.last_called_session = None
-
-  def is_eot(self, tokid: int):
-    return self.model.is_eos_token(tokid)
+    self.eos_token = Llama.token_eos()
+    self.bos_token = Llama.token_bos()
 
   def eval(self, tokens: List[int]) -> torch.Tensor:
     self.model.eval(tokens)
-    return torch.tensor(self.model.logits)
+    return torch.from_numpy(self.model._scores[-1, :])
 
-  def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
-    if self.tokenizer:
-      return self.tokenizer.tokenize(text, add_special_tokens=add_special_tokens)
-    else:
-      return self.model.tokenize(text)
-
-  def detokenize(self, tokens: List[int]) -> str:
-    if self.tokenizer:
-      return self.tokenizer.detokenize(tokens)
-    else:
-      return self.model.detokenize(tokens)
-
-  def enter_session(self, session: "CTransformersSession"):
+  def enter_session(self, session: "LlamaCppSession"):
     if self.last_called_session is None:
       self.last_called_session = weakref.ref(session)
       return
     last_called_session = self.last_called_session()
     if session == last_called_session:
       return
     elif last_called_session is not None:
-      last_called_session._logits = self.load_logits_from_model()
+      last_called_session._logits = self.load_logits_from_llama()
       last_called_session._state = self.model.save_state()
     if session._state is not None:
-      self.model.set_state(session._state)
+      self.model.load_state(session._state)
     self.last_called_session = weakref.ref(session)
 
-  def load_logits_from_model(self) -> torch.Tensor:
+  def load_logits_from_llama(self) -> torch.Tensor:
     return torch.Tensor(self.model.eval_logits[-1])
 
-  def clone_state(self, session: "CTransformersSession") -> CTransformersState:
+  def clone_state(self, session: "LlamaCppSession") -> LlamaState:
     self.enter_session(session)
-    return self.model.clone_state()
+    return self.model.save_state()
 
-  def set_state(self, session: "CTransformersSession", state: Optional[CTransformersState]):
+  def set_state(self, session: "LlamaCppSession", state: Optional[LlamaState]):
     self.enter_session(session)
     self.model.reset()
     if state is not None:
-      self.model.set_state(state)
+      self.model.load_state(state)
 
 
-class CTransformersSession(
-  LLMGenerationSessionForRawText["CTransformersModel", CTransformersState, torch.Tensor]
+class LlamaCppSession(
+  LLMGenerationSessionForRawText["LlamaCppModel", LlamaState, torch.Tensor]
 ):
   """
   Session for llama.cpp model.
   """
 
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
 
-    def load_model(llm: CTransformersModel):
-      return CTransformersWrapper(model_path=llm._model_path, **llm._model_kwargs)
+    def load_model(llm: LlamaCppModel):
+      return LlamaWrapper(model_path=llm._model_path, **llm._model_kwargs)
 
     self._model = self._ld._get_model_internal(self._llm, load_model)
-
     self._logits = None
     self._state = None
     self._next_token = None
 
   def _eval(self, token: int):
     return self._model.eval([token])
 
@@ -129,113 +104,132 @@
 
   def next_token_logits(self) -> List[float]:
     return self._next_token_logits_raw().tolist()
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
-  def set_state(self, state: Optional[CTransformersState]):
+  def set_state(self, state: Optional[LlamaState]):
     self._model.set_state(self, state)
     if state == None:
       self._logits = None
     else:
-      self._logits = self._model.load_logits_from_model()
+      self._logits = self._model.load_logits_from_llama()
 
-  def clone_state(self) -> CTransformersState:
+  def clone_state(self) -> LlamaState:
     return self._model.clone_state(self)
 
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
-    return self._model.tokenize(text, add_special_tokens=add_special_tokens)
+    return self._model.tokenizer.encode(text)
 
   def decode(self, tokens: List[int]) -> str:
-    return self._model.detokenize(tokens)
+    return self._model.tokenizer.decode(tokens)
+
+  def _on_first_inject(self):
+    self._model.model.reset()
+    self._eval(self._model.bos_token)
 
   def _infer(self, end: Optional[Union[str, int]],
              args: InferArgs) -> Generator[RespInfer, None, None]:
     self._model.enter_session(self)
 
     generated = ""
-    ctx: List[int] = []
-    buffered_tokens: List[int] = []
-    stops_at_eot = (
-      (isinstance(end, str) and len(end) == 0) or
-      (isinstance(end, int) and self._model.is_eot(end))
-    )
+    buffered_tokens: Optional[BytesDictBufferedToken] = None
+
+    if isinstance(end, str):
+      if len(end) == 0:
+        end = self._model.eos_token
+      elif args.min_new_tokens > 0:
+        endtoks = self.tokenize(end)
+        print(endtoks)
+        assert len(endtoks) == 1
+        end = endtoks[0]
 
     if self._logits is None:
-      raise ValueError("no prompt provided for CTransformersModel")
+      raise ValueError("no prompt provided for LlamaCppModel")
 
     for i in range(args.max_new_tokens):
-      strip_left = None
+      strip_left: Optional[str] = None
 
       if i == 0 and self._next_token is not None:
-        tokid, tokstr = self._next_token
-
-        for logits_tokstr, logits_tokid in self._model.vocab:
-          if not logits_tokstr.startswith(tokstr):
-            self._logits[logits_tokid] = -inf
+        for logits_tokid in self._model.tokenizer.tokens_starting_with(
+          self._next_token[0]
+        ):
+          self._logits[logits_tokid] = -inf
 
         if self._logits.isinf().all():
           # we don't need to heal tokens because no token that begins with _next_token
-          self._logits = self._eval(tokid)
+          self._logits = self._eval(self._next_token[0])
         else:
-          strip_left = tokstr
+          strip_left = self._next_token[1]
 
         self._next_token = None
 
-      if not stops_at_eot:  # no early endoftext
-        self._logits[0] = -inf
+      if end != self._model.eos_token:  # no early endoftext
+        self._logits[self._model.eos_token] = -inf
+      elif args.min_new_tokens > 0 and i < args.min_new_tokens:
+        self._logits[end] = -inf
 
-      tokid = sampling.sample(self._logits, args, ctx)
-      ctx.append(tokid)
+      tokid = sampling.sample(self._logits, args, self._model.model.eval_tokens)
 
-      if stops_at_eot and self._model.is_eot(tokid):
+      if tokid == end:  # implies end is int
         break
-      elif tokid in self._model.buffered_token_head:
-        buffered_tokens.append(tokid)
-      else:
-        if buffered_tokens:
-          tokstr = self._model.detokenize(buffered_tokens + [tokid])
-          buffered_tokens = []
+
+      tokstr: Optional[str] = None
+
+      if buffered_tokens is None:
+        tokstr_or_buffered = self._model.tokenizer.decode_once(tokid)
+
+        if isinstance(tokstr_or_buffered, str):
+          tokstr = tokstr_or_buffered
         else:
-          tokstr = self._model.detokenize([tokid])
+          buffered_tokens = tokstr_or_buffered
+      else:
+        tokstr = buffered_tokens.add_token_id(tokid)
 
-        if strip_left and tokstr.startswith(tokstr):
+      if tokstr is not None:
+        if strip_left and tokstr.startswith(strip_left):
           tokstr = tokstr[len(strip_left):]
 
         self._next_token = (tokid, tokstr)
 
         generated += tokstr
         if isinstance(end, str) and end and generated.endswith(end):
           generated = generated[:-len(end)]
           break
 
         yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
 
+        buffered_tokens = None
+
       self._logits = self._eval(tokid)
 
+    if buffered_tokens:
+      tokstr = buffered_tokens.flush()
+      generated += tokstr
+      yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
     yield RespInfer(tokid=-1, tokstr="", running_infer=generated)
 
   # Wrapper for public functions to flush the old session states
 
   def inject(self, *a, **k):
     self._model.enter_session(self)
     return LLMGenerationSessionForRawText.inject(self, *a, **k)
 
   def flush_token(self, *a, **k):
     self._model.enter_session(self)
     return LLMGenerationSessionForRawText.inject(self, *a, **k)
 
 
-class CTransformersModel(LLM[CTransformersSession]):
+class LlamaCppModel(LLM[LlamaCppSession]):
   """
   llama.cpp model.
   """
 
-  Session = CTransformersSession
+  Session = LlamaCppSession
 
   def __init__(self, model_path: str, **model_kwargs):
     self._model_path = model_path
     self._model_kwargs = model_kwargs
 
   def session(self, **kwargs):
-    return CTransformersSession(self, **kwargs)
+    return LlamaCppSession(self, **kwargs)
```

### Comparing `langdash-1.3.1a0/langdash/models/mock.py` & `langdash-1.3.2b0/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/models/rwkv_cpp.py` & `langdash-1.3.2b0/langdash/models/rwkv_cpp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Generator, List, Optional, Tuple, Union, Dict, Any
 from math import inf
 from dataclasses import dataclass
 import copy
+import os
+import sys
+import torch
+import tokenizers
 
 from langdash.response import RespInfer
 from langdash.llm import LLM
 from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
 from langdash.infer import InferArgs
 import langdash.sampling as sampling
 import langdash.models._bpe as bpe
-
-import os
-import sys
-import torch
-import tokenizers
+from ._tokenizer.tokenizer import Tokenizer, BufferedToken
+from ._tokenizer.rwkv_20b_tokenizer import Rwkv20BTokenizer
 
 _rwkv_lib: Optional[str] = None
 _rwkv_cpp_folder: Optional[str] = None
 
 RWKV_CPP_COMMIT_DEFAULT = "82c4ac78f4d10ef1af87104fc051ea2119eaaddf"
 RWKV_CPP_COMMIT = os.environ.get(
   "LANGDASH_RWKV_CPP_COMMIT", RWKV_CPP_COMMIT_DEFAULT
@@ -48,20 +49,21 @@
     if not do_install:
       raise ImportError("rwkv.cpp is not installed")
     if git is None:
       raise ImportError("git is needed for compiling rwkv.cpp")
 
     os.makedirs(_rwkv_cpp_folder, exist_ok=True)
 
-    subprocess.check_call(
-      [
-        git, "clone", "--recursive", "https://github.com/saharNooby/rwkv.cpp",
-        _rwkv_cpp_folder
-      ]
-    )
+    if not os.path.isdir(_rwkv_cpp_folder):
+      subprocess.check_call(
+        [
+          git, "clone", "--recursive", "https://github.com/saharNooby/rwkv.cpp",
+          _rwkv_cpp_folder
+        ]
+      )
     subprocess.check_call(
       [git, "checkout", RWKV_CPP_COMMIT], cwd=_rwkv_cpp_folder
     )
     subprocess.check_call([git, "submodule", "update"], cwd=_rwkv_cpp_folder)
 
   elif git is not None:
     current_commit = subprocess.check_output(
@@ -121,61 +123,57 @@
 @dataclass
 class RwkvCppState(LLMState):
   _logits: Optional[torch.Tensor] = None
   _state: Optional[torch.Tensor] = None
   _next_token: Optional[Tuple[int, str]] = None
 
 
-@dataclass
-class RwkvCppExtras:
-  tokenizer: Any
-  vocab: Dict[str, int]
+class RwkvCppWrapper:
+
+  def __init__(self, llm: "RwkvCppModel"):
+    assert _rwkv_lib is not None
+    self.model = rwkv_cpp_model.RWKVModel(
+      rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib), llm._model_path
+    )
+    if llm._tokenizer_type == "20B":
+      tokenizer = tokenizers.Tokenizer.from_file(llm._tokenizer_path)
+    elif llm._tokenizer_type == "world":
+      tokenizer = rwkv_tokenizer.TRIE_TOKENIZER(llm._tokenizer_path)
+    else:
+      raise ValueError(f"unknown tokenizer type {llm._tokenizer_type}")
+    vocab = {
+      bpe.decode(logits_tokstr): logits_tokid
+      for logits_tokstr, logits_tokid in tokenizer.get_vocab().items()
+    }
+    self.tokenizer = Rwkv20BTokenizer(tokenizer, vocab)
+    self.eos_token = 0
+
+  def eval(self, tokid, state):
+    return self.model.eval(tokid, state)
 
 
 class RwkvCppSession(
   LLMGenerationSessionForRawText["RwkvCppModel", RwkvCppState, torch.Tensor]
 ):
   """
   Session for rwkv.cpp model.
   """
 
-  _rwkv: rwkv_cpp_model.RWKVModel
-  _tokenizer: tokenizers.Tokenizer
-
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
 
     def load_model(llm: RwkvCppModel):
-      assert _rwkv_lib is not None
-      model = rwkv_cpp_model.RWKVModel(
-        rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib), llm._model_path
-      )
-      if llm._tokenizer_type == "20B":
-        tokenizer = tokenizers.Tokenizer.from_file(llm._tokenizer_path)
-      elif llm._tokenizer_type == "world":
-        tokenizer = rwkv_tokenizer.TRIE_TOKENIZER(llm._tokenizer_path)
-      else:
-        raise ValueError(f"unknown tokenizer type {llm._tokenizer_type}")
-      extras = RwkvCppExtras(
-        tokenizer=tokenizer,
-        vocab={
-          bpe.decode(logits_tokstr): logits_tokid
-          for logits_tokstr, logits_tokid in tokenizer.get_vocab().items()
-        }
-      )
-      return model, extras
+      return RwkvCppWrapper(llm)
 
-    self._rwkv, self._extras = self._ld._get_model_internal(
-      self._llm, load_model
-    )
+    self._model = self._ld._get_model_internal(self._llm, load_model)
     self._logits, self._state = None, None
     self._next_token = None
 
   def _eval(self, tokid: int) -> torch.Tensor:
-    self._logits, self._state = self._rwkv.eval(tokid, self._state)
+    self._logits, self._state = self._model.eval(tokid, self._state)
     return self._logits
 
   def set_state(self, state: Optional[RwkvCppState]):
     if state is None:
       self._logits, self._state = None, None
       self._next_token = None
     else:
@@ -187,111 +185,114 @@
     return RwkvCppState(
       _logits=copy.deepcopy(self._logits),
       _state=copy.deepcopy(self._state),
       _next_token=self._next_token,
     )
 
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
-    return self._extras.tokenizer.encode(
+    return self._model.tokenizer.encode(
       text, add_special_tokens=add_special_tokens
-    ).ids
+    )
 
   def decode(self, tokids: List[int]) -> str:
-    return self._extras.tokenizer.decode(tokids)
+    return self._model.tokenizer.decode(tokids)
 
   def _next_token_logits_raw(self):
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
-      logits, _ = self._rwkv.eval(self._next_token[0], self._state)
+      logits, _ = self._model.eval(self._next_token[0], self._state)
     return logits
 
   def next_token_logits(self) -> List[float]:
     return self._next_token_logits_raw().tolist()
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
   def _infer(self, end: Optional[Union[str, int]],
              args: InferArgs) -> Generator[RespInfer, None, None]:
     generated = ""
-    ctx: List[int] = []
-    buffered_tokens: List[int] = []
-
-    assert args.min_new_tokens >= 0, "min_new_tokens must be at least 0"
+    buffered_tokens: Optional[BytesDictBufferedToken] = None
+    ctx = []
 
     if isinstance(end, str):
       if len(end) == 0:
-        end = 0
+        end = self._model.eos_token
       elif args.min_new_tokens > 0:
         endtoks = self.tokenize(end)
         assert len(endtoks) == 1
         end = endtoks[0]
 
     if self._logits is None:
-      raise ValueError("no prompt provided for RwkvCppModel")
+      raise ValueError("no prompt provided for LlamaCppModel")
 
     for i in range(args.max_new_tokens):
-      strip_left = None
+      strip_left: Optional[str] = None
 
       if i == 0 and self._next_token is not None:
-        tokid, tokstr = self._next_token
-
-        for logits_tokstr, logits_tokid in self._extras.vocab.items():
-          if not logits_tokstr.startswith(tokstr):
-            self._logits[logits_tokid] = -inf
+        for logits_tokid in self._model.tokenizer.tokens_starting_with(
+          self._next_token[0]
+        ):
+          self._logits[logits_tokid] = -inf
 
         if self._logits.isinf().all():
           # we don't need to heal tokens because no token that begins with _next_token
-          self._logits = self._eval(tokid)
+          self._logits = self._eval(self._next_token[0])
         else:
-          strip_left = tokstr
+          strip_left = self._next_token[1]
 
         self._next_token = None
 
-      if end != 0:  # no early endoftext
-        self._logits[0] = -inf
+      if end != self._model.eos_token:  # no early endoftext
+        self._logits[self._model.eos_token] = -inf
       elif args.min_new_tokens > 0 and i < args.min_new_tokens:
         self._logits[end] = -inf
 
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
 
       if tokid == end:  # implies end is int
         break
 
-      tokstr = self._extras.tokenizer.decode([tokid])
+      tokstr: Optional[str] = None
 
-      if "\ufffd" in tokstr:
-        buffered_tokens.append(tokid)
-        self._next_token = (tokid, "")
-      else:
-        if buffered_tokens:
-          tokstr = self._extras.tokenizer.decode(buffered_tokens)
-          tokstr += self._extras.tokenizer.decode([tokid])
-          buffered_tokens.clear()
+      if buffered_tokens is None:
+        tokstr_or_buffered = self._model.tokenizer.decode_once(tokid)
+
+        if isinstance(tokstr_or_buffered, str):
+          tokstr = tokstr_or_buffered
         else:
-          if strip_left and tokstr.startswith(strip_left):
-            tokstr = tokstr[len(strip_left):]
+          buffered_tokens = tokstr_or_buffered
+      else:
+        tokstr = buffered_tokens.add_token_id(tokid)
+
+      if tokstr is not None:
+        if strip_left and tokstr.startswith(strip_left):
+          tokstr = tokstr[len(strip_left):]
 
         self._next_token = (tokid, tokstr)
 
         generated += tokstr
         if isinstance(end, str) and end and generated.endswith(end):
           generated = generated[:-len(end)]
           break
 
         yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
 
+        buffered_tokens = None
+
       self._logits = self._eval(tokid)
 
     if buffered_tokens:
-      generated += self._extras.tokenizer.decode(buffered_tokens)
+      tokstr = buffered_tokens.flush()
+      generated += tokstr
+      yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
     yield RespInfer(tokid=-1, tokstr="", running_infer=generated)
 
 
 class RwkvCppModel(LLM[RwkvCppSession]):
   """
   rwkv.cpp model
   """
```

### Comparing `langdash-1.3.1a0/langdash/models/sentence_transformers.py` & `langdash-1.3.2b0/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/models/transformers.py` & `langdash-1.3.2b0/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/response.py` & `langdash-1.3.2b0/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/sampling.py` & `langdash-1.3.2b0/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/search/embedding_search.py` & `langdash-1.3.2b0/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/search/engine.py` & `langdash-1.3.2b0/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash/search/multichoice_search.py` & `langdash-1.3.2b0/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/langdash.egg-info/PKG-INFO` & `langdash-1.3.2b0/langdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.3.1a0
+Version: 1.3.2b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.3.1a0/langdash.egg-info/SOURCES.txt` & `langdash-1.3.2b0/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.1a0/setup.py` & `langdash-1.3.2b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,11 +41,11 @@
         # Modules
         "embeddings": ["faiss-cpu"],
 
         # Backend
         "rwkv_cpp": ["tokenizers"],
         "llama_cpp": ["llama-cpp-python==0.1.57"],
         "transformers": ["transformers"],
-        "ctransformers": ["ctransformers @ git+https://git.mysymphony.jp.net/nana/ctransformers.git@daec72c60b"],
+        "ctransformers": ["ctransformers @ git+https://git.mysymphony.jp.net/nana/ctransformers.git@c4eb0c4d59ee85533044ccafaf825c3ba56353d5"],
         "sentence_transformers": ["sentence_transformers"],
     },
 )
```

