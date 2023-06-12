# Comparing `tmp/langdash-1.2.0a1.tar.gz` & `tmp/langdash-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.2.0a1.tar", last modified: Sat Jun 10 03:27:02 2023, max compression
+gzip compressed data, was "langdash-1.3.0a1.tar", last modified: Sun Jun 11 09:43:14 2023, max compression
```

## Comparing `langdash-1.2.0a1.tar` & `langdash-1.3.0a1.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.566714 langdash-1.2.0a1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.2.0a1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.2.0a1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     2854 2023-06-10 03:27:02.566714 langdash-1.2.0a1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1945 2023-06-10 03:20:18.000000 langdash-1.2.0a1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.566714 langdash-1.2.0a1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       64 2023-06-10 03:26:41.000000 langdash-1.2.0a1/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    22279 2023-06-10 03:17:16.000000 langdash-1.2.0a1/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.562714 langdash-1.2.0a1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.2.0a1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1973 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6224 2023-06-07 02:26:23.000000 langdash-1.2.0a1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      793 2023-06-09 06:56:17.000000 langdash-1.2.0a1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.2.0a1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.566714 langdash-1.2.0a1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.2.0a1/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/models/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     7092 2023-06-10 00:53:03.000000 langdash-1.2.0a1/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     9657 2023-06-10 03:09:39.000000 langdash-1.2.0a1/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.2.0a1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     7536 2023-06-10 00:53:03.000000 langdash-1.2.0a1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.2.0a1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2741 2023-06-10 03:12:00.000000 langdash-1.2.0a1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.562714 langdash-1.2.0a1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.2.0a1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1093 2023-06-09 18:58:51.000000 langdash-1.2.0a1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.2.0a1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.2.0a1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-10 03:27:02.566714 langdash-1.2.0a1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2854 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1239 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      167 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-10 03:27:02.000000 langdash-1.2.0a1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-10 03:27:02.566714 langdash-1.2.0a1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1560 2023-06-07 02:26:23.000000 langdash-1.2.0a1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:43:14.388601 langdash-1.3.0a1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.0a1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.0a1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     2854 2023-06-11 09:43:14.388601 langdash-1.3.0a1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1945 2023-06-10 03:20:18.000000 langdash-1.3.0a1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:43:14.384602 langdash-1.3.0a1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-11 09:42:49.000000 langdash-1.3.0a1/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:43:14.388601 langdash-1.3.0a1/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.0a1/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14690 2023-06-11 03:43:22.000000 langdash-1.3.0a1/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8091 2023-06-11 03:43:22.000000 langdash-1.3.0a1/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.0a1/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:43:14.384602 langdash-1.3.0a1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.0a1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1967 2023-06-11 03:43:22.000000 langdash-1.3.0a1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6224 2023-06-07 02:26:23.000000 langdash-1.3.0a1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      777 2023-06-11 03:43:22.000000 langdash-1.3.0a1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.0a1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.0a1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:43:14.388601 langdash-1.3.0a1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.0a1/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.3.0a1/langdash/models/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7092 2023-06-10 00:53:03.000000 langdash-1.3.0a1/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.0a1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9918 2023-06-11 04:47:55.000000 langdash-1.3.0a1/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.3.0a1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7534 2023-06-10 07:12:57.000000 langdash-1.3.0a1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.0a1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2741 2023-06-10 03:12:00.000000 langdash-1.3.0a1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:43:14.384602 langdash-1.3.0a1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.0a1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1098 2023-06-11 03:43:22.000000 langdash-1.3.0a1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.0a1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.0a1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-11 09:43:14.388601 langdash-1.3.0a1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2854 2023-06-11 09:43:14.000000 langdash-1.3.0a1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1304 2023-06-11 09:43:14.000000 langdash-1.3.0a1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-11 09:43:14.000000 langdash-1.3.0a1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      167 2023-06-11 09:43:14.000000 langdash-1.3.0a1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-11 09:43:14.000000 langdash-1.3.0a1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-11 09:43:14.388601 langdash-1.3.0a1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1560 2023-06-07 02:26:23.000000 langdash-1.3.0a1/setup.py
```

### Comparing `langdash-1.2.0a1/LICENSE.txt` & `langdash-1.3.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/PKG-INFO` & `langdash-1.3.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.2.0a1
+Version: 1.3.0a1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.2.0a1/README.md` & `langdash-1.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/chains.py` & `langdash-1.3.0a1/langdash/chains/chains.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from dataclasses import dataclass
 from collections import OrderedDict
-from typing import Generator, Dict, Any, List, Union, Optional, Type, Tuple, FrozenSet, TYPE_CHECKING, cast
+from typing import Generator, Dict, Any, List, Union, Optional, Type, Tuple, FrozenSet, Callable, TYPE_CHECKING, cast
 import re
-import random
 import copy
 import warnings
-from weakref import WeakKeyDictionary
-from math import inf
 
 from langdash.response import Response, RespInfer, RespInject, RespReturns
-from langdash.infer import InferArgs
+from .nodes import LDNode, LDText, LDFormatArg, LDArg, LDReturns, LDChoice, LDRepeat
+from .typing import Type, TypeDict
 
 if TYPE_CHECKING:
   from langdash.core import Langdash
   from langdash.llm_session import LLMGenerationSession, LLMState
 
 RE_FIRST_CONST = re.compile(r"^((?:[^{]|{{)+)")
 RE_IDENT = re.compile(r"^({[a-zA-Z_][a-zA-Z0-9_]*})")
 RE_FORMAT_ARG = re.compile(r"^({[^}]+})")
 
 LDNodeGenerator = Generator[Response, None, None]
 LDNodeArgs = Dict[str, Any]
 LDNodeArgsFrozen = FrozenSet[Tuple[str, Any]]
-TypeDict = Dict[str, Type]
 
 
 @dataclass(frozen=True)
 class CalledChain:
   """
   Data class used to store info about nodes previously called.
   
@@ -209,15 +206,15 @@
         text = ""
         for resp in generator:
           assert isinstance(resp, RespInfer)
           text = resp.running_infer
           if resp.tokid != -1:
             result.completion_tokens += 1
           else:
-            result.returns[key].append(text)
+            result.returns[node._append_target].append(text)
             text = ""
 
       else:
         for resp in generator:
           if isinstance(resp, RespInject):
             result.prompt_tokens += resp.tokens_counter
           else:
@@ -459,292 +456,7 @@
   prompt_tokens: int
   completion_tokens: int
 
   def __init__(self):
     self.returns = {}
     self.prompt_tokens = 0
     self.completion_tokens = 0
-
-
-class LDNode:
-  """ Base class for langdash nodes. """
-
-  def __init__(self, ld: "Langdash"):
-    self._ld = ld
-
-  def __call__(
-    self, session: "LLMGenerationSession", args: LDNodeArgs
-  ) -> LDNodeGenerator:
-    raise NotImplementedError("__call__")
-
-
-class LDText(LDNode):
-  """ Constant text node """
-
-  def __init__(
-    self, ld: "Langdash", text: str, add_special_tokens: bool = False
-  ):
-    super().__init__(ld)
-    self._text = text
-    self._add_special_tokens = add_special_tokens
-
-  def __repr__(self):
-    return f"<Text>\n{self._text}\n</Text>"
-
-  def __call__(
-    self, session: "LLMGenerationSession", args: LDNodeArgs
-  ) -> LDNodeGenerator:
-    tokens_counter = session.inject(
-      self._text, add_special_tokens=self._add_special_tokens
-    )
-    yield RespInject(tokens_counter=tokens_counter)
-
-
-class LDFormatArg(LDNode):
-  """ Format argument node """
-
-  def __init__(self, ld: "Langdash", text: str):
-    super().__init__(ld)
-    self._text = text
-
-  def __repr__(self):
-    return f"<FormatArgs>\n{self._text}\n</FormatArgs>"
-
-  def __call__(
-    self, session: "LLMGenerationSession", args: LDNodeArgs
-  ) -> LDNodeGenerator:
-    tokens_counter = session.inject(
-      self._text.format(globals=session.global_args, **args)
-    )
-    yield RespInject(tokens_counter=tokens_counter)
-
-
-class LDArg(LDNode):
-  """ Argument node """
-
-  def __init__(
-    self, ld: "Langdash", arg: str, padleft: str = "", padright: str = ""
-  ):
-    super().__init__(ld)
-    self._arg = arg
-    self._padleft = padleft
-    self._padright = padright
-
-  def __repr__(self):
-    return f"<Arg arg={self._arg}>"
-
-  def __call__(
-    self, session: "LLMGenerationSession", args: LDNodeArgs
-  ) -> LDNodeGenerator:
-    s = ""
-    s += self._padleft
-    if self._arg in args:
-      s += str(args[self._arg])
-    else:
-      s += str(session.global_args[self._arg])
-    s += self._padright
-    tokens_counter = session.inject(s)
-    yield RespInject(tokens_counter=tokens_counter)
-
-
-class LDReturns(LDNode):
-  """ Return node """
-
-  def __init__(
-    self,
-    ld: "Langdash",
-    returns: str,
-    end: Optional[Union[str, int]],
-    padleft: str = "",
-    infer_args: Optional[InferArgs] = None
-  ):
-    super().__init__(ld)
-    self._returns = returns
-    self._end = end
-    self._padleft = padleft
-    self._infer_args = infer_args
-
-  def __repr__(self):
-    return f"<Returns arg={self._returns}>"
-
-  def __call__(
-    self, session: "LLMGenerationSession", args: LDNodeArgs
-  ) -> LDNodeGenerator:
-    for i, respinfer in enumerate(
-      session.infer(end=self._end, args=self._infer_args)
-    ):
-      if i == 0:
-        if self._padleft and respinfer.tokstr.startswith(self._padleft):
-          respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
-      elif respinfer.tokid == -1:  # end
-        if self._padleft and respinfer.running_infer.startswith(self._padleft):
-          respinfer.running_infer = respinfer.running_infer[len(self._padleft):]
-      yield respinfer
-
-
-@dataclass(frozen=True)
-class _LDChoiceTokensCache:
-  choices_tokens: List[List[int]]
-  heal_prefix: str
-
-
-class LDChoice(LDNode):
-  """ Choice node """
-
-  def __init__(
-    self,
-    ld: "Langdash",
-    returns: str,
-    choices: List[str],
-    padleft: str = "",
-    padright: str = "",
-    argmax: bool = False
-  ):
-    super().__init__(ld)
-    self._returns = returns
-    self._choices = choices
-    self._padleft = padleft
-    self._padright = padright
-    self._argmax = argmax
-
-    self._choices_preprocessed = [
-      f"{self._padleft}{choice}{self._padright}" for choice in self._choices
-    ]
-    self._token_cache: WeakKeyDictionary[
-      str, _LDChoiceTokensCache] = WeakKeyDictionary()
-
-  def __repr__(self):
-    return f"<Choices {self._returns}>"
-
-  def _get_token_cache(
-    self, session: "LLMGenerationSession", heal_prefix: str
-  ) -> _LDChoiceTokensCache:
-    try:
-      cache = self._token_cache[session]
-      if cache.heal_prefix == heal_prefix:
-        return cache
-    except KeyError:
-      pass
-    cache = _LDChoiceTokensCache(
-      choices_tokens=[
-        session.tokenize(heal_prefix + text)
-        for text in self._choices_preprocessed
-      ],
-      heal_prefix=heal_prefix
-    )
-    self._token_cache[session] = cache
-    return cache
-
-  def __call__(
-    self, session: "LLMGenerationSession", args: LDNodeArgs
-  ) -> LDNodeGenerator:
-    from langdash.llm_session import LLMGenerationSessionForRawText
-
-    heal_prefix: str = ""
-    if session.token_healing and \
-      isinstance(session, LLMGenerationSessionForRawText) and \
-      session._next_token is not None:
-      heal_prefix = session._next_token[1]
-      session._next_token = None
-
-    cache = self._get_token_cache(session, heal_prefix)
-    choices_tokens: List[Tuple[int, List[int]]] = [
-      (i, list(reversed(tokens)))
-      for i, tokens in enumerate(cache.choices_tokens)
-    ]
-
-    while len(choices_tokens) > 1:
-      probs = session.next_token_probs()
-
-      if self._argmax:
-        tokid = -1
-        tokid_prob = -inf
-        for _, tokens in choices_tokens:
-          cur_tokid = tokens[-1]
-          if probs[cur_tokid] > tokid_prob:
-            tokid = cur_tokid
-            tokid_prob = probs[cur_tokid]
-      else:
-        cur_choice_tokens = []
-        cur_choice_weights = []
-        for _, tokens in choices_tokens:
-          tokid = tokens[-1]
-          cur_choice_tokens.append(tokid)
-          cur_choice_weights.append(probs[tokid])
-        tokid = random.choices(cur_choice_tokens, weights=cur_choice_weights)[0]
-
-      session.inject(tokid)
-
-      old_choices_tokens = choices_tokens
-      choices_tokens = []
-      for i, tokens in old_choices_tokens:
-        if tokens[-1] == tokid:
-          tokens.pop()
-          choices_tokens.append((i, tokens))
-
-    choice, remaining = choices_tokens.pop()
-    for tokid in reversed(remaining):
-      session.inject(tokid)
-    yield RespInfer(-1, "", self._choices[choice])
-    yield RespInject(tokens_counter=len(cache.choices_tokens[choice]))
-
-
-class LDRepeat(LDNode):
-  """ Repeat node """
-
-  def __init__(
-    self,
-    ld: "Langdash",
-    subchain: LDChain,
-    append_source: str,
-    append_target: str,
-    end: str = "",
-    max_len: int = -1,
-    end_threshold: float = 0.5
-  ):
-    super().__init__(ld)
-    assert subchain._ld == ld
-    self._subchain = subchain
-    self._append_source = append_source
-    self._append_target = append_target
-    self._end = end
-    self._max_len = max_len
-    self._end_threshold = end_threshold
-
-  def __call__(
-    self, session: "LLMGenerationSession", args: LDNodeArgs
-  ) -> LDNodeGenerator:
-    if self._end:
-      end_toks = session.tokenize(self._end)
-      assert len(end_toks) == 1, "only supports 1 end token"
-      end_tok = end_toks[0]
-    else:
-      end_tok = 0
-    append_resp = RespReturns(key=self._append_target)
-
-    i = 0
-    while True:
-      in_append_source = False
-      for resp in self._subchain.stream(session, args=args):
-        if isinstance(resp, RespReturns):
-          if resp.key == self._append_source:
-            in_append_source = True
-            yield append_resp
-          else:
-            in_append_source = False
-            yield resp
-        elif isinstance(resp, RespInfer):
-          if resp.tokid == -1:
-            yield resp
-            if in_append_source:
-              in_append_source = False
-        else:
-          yield resp
-          in_append_source = False
-
-      prob_dist = session.next_token_probs()
-      if prob_dist[end_tok] > self._end_threshold:
-        break
-
-      i += 1
-      if i == self._max_len:
-        break
```

### Comparing `langdash-1.2.0a1/langdash/classify/token_qa.py` & `langdash-1.3.0a1/langdash/classify/token_qa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, List, Tuple, Dict, Optional, cast
+from typing import Union, List, Tuple, Dict, Optional
 from langdash.chains import LDChainCached, LDResult, LDNodeArgs
 from langdash.llm_session import LLMGenerationSession
 
 
 class TokenQA:
   _classes_tok: Dict[str, List[int]]
```

### Comparing `langdash-1.2.0a1/langdash/core.py` & `langdash-1.3.0a1/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/infer.py` & `langdash-1.3.0a1/langdash/infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-import warnings
 
 
 @dataclass
 class InferArgs:
   """
   Data class for inference arguments.
```

### Comparing `langdash-1.2.0a1/langdash/llm.py` & `langdash-1.3.0a1/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/llm_session.py` & `langdash-1.3.0a1/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/models/_bpe.py` & `langdash-1.3.0a1/langdash/models/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/models/llama_cpp.py` & `langdash-1.3.0a1/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/models/mock.py` & `langdash-1.3.0a1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/models/rwkv_cpp.py` & `langdash-1.3.0a1/langdash/models/rwkv_cpp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generator, List, Optional, Tuple, Union, Dict
+from typing import Generator, List, Optional, Tuple, Union, Dict, Any
 from math import inf
 from dataclasses import dataclass
 import copy
 
 from langdash.response import RespInfer
 from langdash.llm import LLM
 from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
@@ -74,15 +74,18 @@
       subprocess.check_call(
         [git, "checkout", RWKV_CPP_COMMIT], cwd=_rwkv_cpp_folder
       )
       subprocess.check_call([git, "submodule", "update"], cwd=_rwkv_cpp_folder)
       force_recompile = True
 
   if force_recompile:
-    os.unlink(os.path.join(_rwkv_cpp_folder, "CMakeCache.txt"))
+    try:
+      os.unlink(os.path.join(_rwkv_cpp_folder, "CMakeCache.txt"))
+    except FileNotFoundError:
+      pass
 
   if "win32" in sys.platform or "cygwin" in sys.platform:
     file_name = "rwkv.dll"
   elif "darwin" in sys.platform:
     file_name = "librwkv.dylib"
   else:
     file_name = "librwkv.so"
@@ -101,29 +104,34 @@
   sys.path.insert(0, os.path.join(_rwkv_cpp_folder, "rwkv"))
 
 
 _load_rwkv_import()
 
 import rwkv_cpp_model  # type: ignore
 import rwkv_cpp_shared_library  # type: ignore
-import rwkv_tokenizer  # type: ignore
+
+try:
+  import rwkv_tokenizer  # type: ignore
+  _rwkv_tokenizer_available = True
+except ModuleNotFoundError:
+  _rwkv_tokenizer_available = False
 
 sys.path.pop(0)
 
 
 @dataclass
 class RwkvCppState(LLMState):
   _logits: Optional[torch.Tensor] = None
   _state: Optional[torch.Tensor] = None
   _next_token: Optional[Tuple[int, str]] = None
 
 
 @dataclass
 class RwkvCppExtras:
-  tokenizer: Union[tokenizers.Tokenizer, rwkv_tokenizer.TRIE_TOKENIZER]
+  tokenizer: Any
   vocab: Dict[str, int]
 
 
 class RwkvCppSession(
   LLMGenerationSessionForRawText["RwkvCppModel", RwkvCppState, torch.Tensor]
 ):
   """
@@ -232,15 +240,15 @@
 
         for logits_tokstr, logits_tokid in self._extras.vocab.items():
           if not logits_tokstr.startswith(tokstr):
             self._logits[logits_tokid] = -inf
 
         if self._logits.isinf().all():
           # we don't need to heal tokens because no token that begins with _next_token
-          self._logits, self._state = self._rwkv.eval(tokid, self._state)
+          self._logits = self._eval(tokid)
         else:
           strip_left = tokstr
 
         self._next_token = None
 
       if end != 0:  # no early endoftext
         self._logits[0] = -inf
@@ -272,15 +280,15 @@
         generated += tokstr
         if isinstance(end, str) and end and generated.endswith(end):
           generated = generated[:-len(end)]
           break
 
         yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
 
-      self._logits, self._state = self._rwkv.eval(tokid, self._state)
+      self._logits = self._eval(tokid)
 
     if buffered_tokens:
       generated += self._extras.tokenizer.decode(buffered_tokens)
     yield RespInfer(tokid=-1, tokstr="", running_infer=generated)
 
 
 class RwkvCppModel(LLM[RwkvCppSession]):
@@ -299,20 +307,22 @@
     """
     Creates a template for the RWKV language model (using the rwkv.cpp library).
     
     Args:
       model_path (str): Path to the model file.
       tokenizer_path (Optional[str]):
         Path to the tokenizer file.
-        If None is given, the built-in tokenizer will be used.
+        Defaults to `None`. If not set, the built-in tokenizer will be used.
       tokenizer_type (str):
-        Either `"world"` or `"20B"`.
+        The type of tokenizer to use. Either `"world"` for world models or `"20B"` for anything else.
     """
     self._model_path = model_path
     self._tokenizer_type = tokenizer_type
+    if not _rwkv_tokenizer_available and self._tokenizer_type != "20B":
+      raise ValueError("old RWKV tokenizer only supports 20B")
     if tokenizer_path is None:
       builtin_tokenizer_paths = {
         "world": "rwkv/rwkv_vocab_v20230424.txt",
         "20B": "rwkv/20B_tokenizer.json",
       }
       self._tokenizer_path = str(
         os.path.join(
```

### Comparing `langdash-1.2.0a1/langdash/models/sentence_transformers.py` & `langdash-1.3.0a1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/models/transformers.py` & `langdash-1.3.0a1/langdash/models/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     Creates a template for a language model powered by the transformers library.
     
     Args:
       model (Union[str, transformers.PreTrainedModel]):
         The name of the model, or the model class itself.
       tokenizer (Optional[Union[str, transformers.PreTrainedTokenizer]]):
         The name of the tokenizer, or the tokenizer class itself.
-        Defaults to `None`. If not set, the name of the model will be used to detect the tokenizer.
+        Defaults to `None`. If not set, the name of the model will be used to load the tokenizer.
     """
     if tokenizer is None:
       assert isinstance(model, str), "model must be string if tokenizer is None"
       tokenizer = model
     self._model = model
     self._tokenizer = tokenizer
     self._model_kwargs = model_kwargs
```

### Comparing `langdash-1.2.0a1/langdash/response.py` & `langdash-1.3.0a1/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/sampling.py` & `langdash-1.3.0a1/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/search/embedding_search.py` & `langdash-1.3.0a1/langdash/search/embedding_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,14 @@
       self._documents += texts
       self._embds.add(self._embd_session.embed(texts))
 
   def search(
     self,
     text: str,
     max_documents: int = 1
-  ) -> Generator[Tuple[str, float], None, None]:
+  ) -> Generator[Tuple[int, str, float], None, None]:
     embd = self._embd_session.embed([text])
     if max_documents == -1:
       max_documents = len(self._documents)
     D, I = self._embds.search(embd, max_documents)
     for d, i in zip(D[0], I[0]):
       yield i, self._documents[i], d
```

### Comparing `langdash-1.2.0a1/langdash/search/engine.py` & `langdash-1.3.0a1/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash/search/multichoice_search.py` & `langdash-1.3.0a1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.2.0a1/langdash.egg-info/PKG-INFO` & `langdash-1.3.0a1/langdash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.2.0a1
+Version: 1.3.0a1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.2.0a1/langdash.egg-info/SOURCES.txt` & `langdash-1.3.0a1/langdash.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 ./langdash/__init__.py
-./langdash/chains.py
 ./langdash/infer.py
 ./langdash/llm.py
 ./langdash/llm_session.py
 ./langdash/response.py
 ./langdash/sampling.py
 ./langdash/classify/__init__.py
 ./langdash/classify/token_qa.py
@@ -16,26 +15,29 @@
 ./langdash/models/sentence_transformers.py
 ./langdash/models/transformers.py
 ./langdash/search/__init__.py
 ./langdash/search/embedding_search.py
 ./langdash/search/engine.py
 ./langdash/search/multichoice_search.py
 langdash/__init__.py
-langdash/chains.py
 langdash/core.py
 langdash/infer.py
 langdash/llm.py
 langdash/llm_session.py
 langdash/response.py
 langdash/sampling.py
 langdash.egg-info/PKG-INFO
 langdash.egg-info/SOURCES.txt
 langdash.egg-info/dependency_links.txt
 langdash.egg-info/requires.txt
 langdash.egg-info/top_level.txt
+langdash/chains/__init__.py
+langdash/chains/chains.py
+langdash/chains/nodes.py
+langdash/chains/typing.py
 langdash/classify/__init__.py
 langdash/classify/token_qa.py
 langdash/models/__init__.py
 langdash/models/_bpe.py
 langdash/models/llama_cpp.py
 langdash/models/mock.py
 langdash/models/rwkv_cpp.py
```

### Comparing `langdash-1.2.0a1/setup.py` & `langdash-1.3.0a1/setup.py`

 * *Files identical despite different names*

