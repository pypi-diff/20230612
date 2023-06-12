# Comparing `tmp/promptwatch-0.2.1.tar.gz` & `tmp/promptwatch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.2.1.tar", last modified: Sun Jun  4 13:25:55 2023, max compression
+gzip compressed data, was "promptwatch-0.2.2.tar", last modified: Mon Jun 12 10:35:54 2023, max compression
```

## Comparing `promptwatch-0.2.1.tar` & `promptwatch-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.370855 promptwatch-0.2.1/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-04 13:25:55.370697 promptwatch-0.2.1/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.1/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.1/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-04 13:25:55.370897 promptwatch-0.2.1/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.1/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.363488 promptwatch-0.2.1/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.366706 promptwatch-0.2.1/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-06-04 13:23:24.000000 promptwatch-0.2.1/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.1/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.1/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.1/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5459 2023-05-30 20:36:31.000000 promptwatch-0.2.1/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.1/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.369254 promptwatch-0.2.1/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.1/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.1/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    29649 2023-06-04 13:06:19.000000 promptwatch-0.2.1/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.1/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17902 2023-05-31 18:53:06.000000 promptwatch-0.2.1/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.370332 promptwatch-0.2.1/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.1/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.1/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.1/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.1/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1105 2023-05-24 13:30:08.000000 promptwatch-0.2.1/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.367854 promptwatch-0.2.1/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.1/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 10:35:54.114857 promptwatch-0.2.2/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-12 10:35:54.114657 promptwatch-0.2.2/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.2/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.2/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-12 10:35:54.114933 promptwatch-0.2.2/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.2/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 10:35:54.105301 promptwatch-0.2.2/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 10:35:54.109990 promptwatch-0.2.2/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-06-12 10:34:46.000000 promptwatch-0.2.2/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.2/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.2/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.2/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5459 2023-05-30 20:36:31.000000 promptwatch-0.2.2/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.2/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 10:35:54.112872 promptwatch-0.2.2/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.2/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.2/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    30508 2023-06-12 10:18:17.000000 promptwatch-0.2.2/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.2/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17902 2023-06-12 10:33:52.000000 promptwatch-0.2.2/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 10:35:54.114109 promptwatch-0.2.2/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.2/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.2/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.2/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.2/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1105 2023-05-24 13:30:08.000000 promptwatch-0.2.2/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 10:35:54.111426 promptwatch-0.2.2/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-12 10:35:54.000000 promptwatch-0.2.2/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-06-12 10:35:54.000000 promptwatch-0.2.2/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-12 10:35:54.000000 promptwatch-0.2.2/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.2/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-06-12 10:35:54.000000 promptwatch-0.2.2/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-06-12 10:35:54.000000 promptwatch-0.2.2/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.2.1/PKG-INFO` & `promptwatch-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.1
+Version: 0.2.2
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.1/README.md` & `promptwatch-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/setup.py` & `promptwatch-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/caching.py` & `promptwatch-0.2.2/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/client.py` & `promptwatch-0.2.2/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/data_model.py` & `promptwatch-0.2.2/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/decorators.py` & `promptwatch-0.2.2/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/langchain/caching.py` & `promptwatch-0.2.2/src/promptwatch/langchain/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.2.2/src/promptwatch/langchain/langchain_support.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import datetime
 from langchain.prompts.base import BasePromptTemplate
 from langchain.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate, AIMessagePromptTemplate, SystemMessagePromptTemplate, MessagesPlaceholder, BaseMessagePromptTemplate
 from langchain.llms.base import LLM
 from langchain.chat_models.base import BaseChatModel
 from langchain.chains import LLMChain
 from langchain.embeddings.base import Embeddings
-from langchain.schema import HumanMessage, ChatMessage as LangChainChatMessage, AIMessage, SystemMessage, BaseMessage
+from langchain.schema import HumanMessage, ChatMessage as LangChainChatMessage, AIMessage, SystemMessage, BaseMessage 
+from langchain.prompts import ChatMessagePromptTemplate as LangChainChatMessagePromptTemplate
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.agents import initialize_agent, Tool, Agent, BaseSingleActionAgent
 from langchain.tools.base import BaseTool
 from langchain.chains.base import Chain
 
 from langchain.schema import AgentAction, AgentFinish, LLMResult,  Document
 from ..client import Client
@@ -137,28 +138,40 @@
     
 
     def reverse_monkey_patching(self):
         for func in self.monkey_patched_functions:
             #TODO: .. we should restore the state of the things as were before...
             pass
             
-
+        
+    def on_chat_model_start(
+        self,
+        serialized: Dict[str, Any],
+        messages: List[List[BaseMessage]],
+        *,
+        run_id,
+        parent_run_id = None,
+        **kwargs: Any,
+    ) -> Any:
+        self.on_llm_start(serialized, messages, run_id=run_id, parent_run_id=parent_run_id, **kwargs)
     
 
     def on_llm_start(
-        self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
+        self, serialized: Dict[str, Any], prompts: List[str, List[BaseMessage]], **kwargs: Any
     ) -> Any:
         """Run when LLM starts running."""
 
         prompt_template = None
         prompt_input_values=None
         llm_info=None
         info_message=None
         formatted_prompt=None
 
+        
+
         current_llm_chain:LLMChain= self.prompt_watch.get_context(LLM_CHAIN_CONTEXT_KEY)
 
         template_name = self.prompt_watch.get_context(TEMPLATE_NAME_CONTEXT_KEY)
         if template_name:
             prompt_template = PromptWatch.prompt_template_register_cache.get(template_name)
             
         # this should ensure that all the additional data is available in the context
@@ -175,25 +188,32 @@
             if not prompt_template:
                 # lets create anonymous prompt template description
                 prompt_template = create_prompt_template_description(current_llm_chain.prompt)
 
             prompt_input_values = self.prompt_watch.current_activity.inputs
 
             formatted_prompt = self.prompt_watch.get_context(FORMATTED_PROMPT_CONTEXT_KEY)
-            if isinstance(current_llm_chain.prompt,ChatPromptTemplate):
+
+            
+            if prompts and prompts[0] and isinstance(prompts[0][0],LangChainChatMessage):
+                
+                prompts=[convert_chat_messages(prompts_set) for prompts_set in prompts]
+            # this is probably unnecessary now, but keeping it for now
+            elif isinstance(current_llm_chain.prompt,ChatPromptTemplate):
                 if not formatted_prompt:
                     # we need to reformat the prompt so we can get the original values, not the strings
                     formatted_prompt = current_llm_chain.prep_prompts([prompt_input_values])[0][0]
                 if formatted_prompt:
                     #throwing away the original prompt from langchain tracing and replacing it with the original formatted messages
                     prompts = [convert_chat_messages(formatted_prompt.messages)]
             
             
             
             
+            
 
             if prompt_template and prompt_template.prompt_input_params and prompt_input_values:
                 prompt_input_values = {k:v for k,v in prompt_input_values.items() if k in prompt_template.prompt_input_params and (isinstance(v,str) )}
             else:
                 prompt_input_values={k:v for k,v in prompt_input_values.items() if isinstance(v,str)}
 
             if  prompt_template and isinstance(prompt_template.prompt_template,list):
@@ -201,63 +221,63 @@
                 for k, v in non_text_input.items():
                     if v and isinstance(v,list) and isinstance(v[0],ChatMessage):
                         prompt_input_values[k] = v
                     # this should be necessary anymore... keeping it just in case
                     if v and isinstance(v,list) and isinstance(v[0],BaseMessage):
                         prompt_input_values[k] = convert_chat_messages(v)
                         
-
         else:
             info_message="Could not retrieve all the additional information needed to for reproducible prompt execution. Consider registering the prompt template."
 
         if len(prompts)==1:
             
             self.prompt_watch._open_activity(LlmPrompt(
                 prompt= prompts[0], #why we have here more than one prompt?
                 prompt_template=prompt_template,
                 prompt_input_values=prompt_input_values,
                 metadata={"llm":llm_info,**(serialized or {}),**(kwargs or {})} 
                 ))
         elif len(prompts)>1:
-            thoughts = []
+            _prompts = []
             for prompt in prompts:
-                thoughts.append( LlmPrompt(
+                _prompts.append( LlmPrompt(
                             prompt=prompt, #why we have here more than one prompt?
                             prompt_template=prompt_template,
                             prompt_input_values=prompt_input_values,
                             info_message=info_message,
                         ))
             self.prompt_watch._open_activity(ParallelPrompt(
-                    thoughts=thoughts,
+                    prompts=prompts,
                     metadata={**serialized,**kwargs} if serialized and kwargs else (serialized or kwargs),
                     order=self.prompt_watch.current_session.steps_count+1, 
                     session_id=self.prompt_watch.current_session.id,
                     info_message=info_message,
                 )
             )
 
 
 
     
     def on_llm_new_token(self, token: str, **kwargs: Any) -> Any:
         """Run on new LLM token. Only available when streaming is enabled."""
+        pass
 
     
     def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
         """Run when LLM ends running."""
         if len(response.generations)>1:
-            thoughts =  self.prompt_watch.current_activity.thoughts
+            prompts =  self.prompt_watch.current_activity.thoughts
         else:
-            thoughts=[self.prompt_watch.current_activity]
+            prompts=[self.prompt_watch.current_activity]
         
         
         if not self.prompt_watch.current_activity.metadata:
             self.prompt_watch.current_activity.metadata={}
 
-        for thought, generated_responses in zip(thoughts, response.generations):
+        for thought, generated_responses in zip(prompts, response.generations):
             thought.generated = "\n---\n".join([resp.text for resp in generated_responses])
             thought.metadata["generation_info"] = [resp.generation_info for resp in generated_responses] if len(generated_responses)>1 else generated_responses[0].generation_info
 
         if response.llm_output is not None:
             self.prompt_watch.current_activity.metadata["llm_output"]=response.llm_output
             token_usage= response.llm_output.get("token_usage")
             if token_usage and isinstance(token_usage,dict):
@@ -632,14 +652,16 @@
             
                 if isinstance(msg,HumanMessagePromptTemplate):
                     role="user"
                 elif isinstance(msg,AIMessagePromptTemplate):
                     role="assistant"
                 elif isinstance(msg,SystemMessagePromptTemplate):
                     role="system"
+                elif isinstance(msg,LangChainChatMessagePromptTemplate):
+                    role=msg.role
                 if hasattr(msg,"prompt"):
                     if hasattr(msg.prompt,"template"):
                         prompt_template = msg.prompt.template
                     if hasattr(msg.prompt,"input_variables"):
                         msg_input_params = msg.prompt.input_variables
                         if msg_input_params:
                             for param in msg_input_params:
```

### Comparing `promptwatch-0.2.1/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.2.2/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/promptwatch_context.py` & `promptwatch-0.2.2/src/promptwatch/promptwatch_context.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.2.2/src/promptwatch/unit_tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.2.2/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.2.2/src/promptwatch/unit_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch/utils.py` & `promptwatch-0.2.2/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.1/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.2.2/src/promptwatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.1
+Version: 0.2.2
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.1/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.2.2/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

